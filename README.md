📊 E-commerce Sales Dashboard - Power BI

🎯 Overview
Built a comprehensive sales dashboard that transforms raw data into actionable business insights for data-driven decision making.

📂 Data Sources

Details.csv - Product information (ID, Name, Category, Price)
Orders.csv - Transaction data (Order ID, Customer ID, Date, Revenue, Region)


✨ Key Features
Sales Analytics

Revenue trends and growth analysis
Regional sales distribution
Month-over-month comparison

Product Insights

Top-performing products and categories
Profitability analysis
Inventory optimization

Customer Analysis

Purchase behavior patterns
Customer segmentation
Repeat customer tracking

Interactive Elements

Dynamic filters for date, region, category
Drill-down capabilities
KPI cards for quick metrics

🛠️ Technical Skills

TechnologyUsagePower BIDashboard & visualizationPower QueryData cleaning & transformationDAXCustom calculations & measures
Key DAX Measures:

Total Revenue = SUM(Orders[Revenue])

Average Order Value = DIVIDE([Total Revenue], [Total Orders])

Revenue Growth % = DIVIDE([Current Month] - [Previous Month], [Previous Month])


