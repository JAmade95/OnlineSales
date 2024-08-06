Overview
This project involves analysing and visualising online sales data using Power BI. The dataset comprises two files: Orders.csv and Details.csv. The goal is to clean the data, establish relationships, and create an informative dashboard with various visualisations and KPIs.

Data Preparation
Data Cleaning and Transformation
Removing Line Breaks:

Issue: Both Orders.csv and Details.csv files contain unwanted line breaks between rows, which can disrupt data processing.
Solution: Python scripts were used to clean these line breaks, ensuring a continuous and accurate dataset.
Date Standardisation:

Issue: Dates in Orders.csv were recorded in multiple formats (e.g., 10/03/18 and 10-03-2018).
Solution: Dates were standardised to a consistent format (DD-MM-YYYY) to facilitate accurate data analysis and avoid format inconsistencies.
Data Transformation in Power BI
Importing Data:

Data from the cleaned CSV files (Standardized_Orders.csv and Cleaned_Details.csv) was imported into Power BI.
Data Type Changes:

Orders Data:
Order Date: Converted to a Date data type for accurate time-based analysis.
Details Data:
Amount, Profit, and Quantity: Verified and formatted correctly to ensure consistency in calculations.
Creating Relationships:

Primary and Related Tables:
Standardized_Orders was set as the primary table, and Cleaned_Details was linked as the related table using Order ID to establish a one-to-many relationship.

Cross Filter Direction:
Set to "Both" to allow filtering in both directions between the two tables, providing a more flexible data analysis experience.

Power BI Dashboard
KPI Cards
Total Sales: Displays the total revenue generated from all orders.
Total Orders: Shows the count of all orders placed.
Average Order Value: Calculates the average value per order.
Total Profit: Summarises the total profit made from sales.

Visualisations

Tree Map: Sales Distribution by Category
Purpose: Provides a visual breakdown of sales across different categories, highlighting the proportion of each category's contribution to total sales.

Stacked Column Chart: Sales and Profit by Category
Purpose: Illustrates sales and profit distribution across various categories, with different colours representing sales and profit.

Stacked Area Chart: Monthly Order Distribution by Payment Mode
Purpose: Shows the trend of order quantities over months, segmented by payment mode. This visual helps identify seasonal patterns and the popularity of different payment methods.

Donut Chart: Amount by Payment Mode
Purpose: Displays the total amount of sales segmented by payment mode, giving a quick overview of how sales are distributed across different payment options.

Bar Chart: Order Quantity by Payment Mode
Purpose: Represents the quantity of orders placed through various payment modes, allowing for comparison of order volumes across different payment methods.

Date Range Slicer
Purpose:
Allows users to filter data based on a custom date range, facilitating more granular analysis of sales and orders over specific periods.

Conclusion
This project demonstrates the process of cleaning, transforming, and visualising online sales data. The dashboard provides key insights through KPI cards and various visualisations, helping users understand sales performance and payment trends effectively.