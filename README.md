# Tailwind Traders Power BI Dashboard

## Overview
This project presents an in-depth analysis of Tailwind Traders' sales, purchases, and profit data using Power BI and Excel. By leveraging advanced data transformation and visualization techniques, this dashboard enables executive-level insights into key performance indicators (KPIs) such as revenue, profit margins, and purchasing trends. The dashboard is designed to provide a holistic view of business performance, allowing stakeholders to make data-driven decisions efficiently.

## Business Objective
The primary goal of this project was to provide actionable insights into Tailwind Traders' financial and operational metrics. Through the integration of various datasets and the creation of meaningful relationships, this dashboard supports decision-makers in understanding regional sales performance, supplier engagement, and profit trends. The project emphasizes data accuracy, clear reporting, and easy navigation across different sections of the business.

## Project Workflow

1. **Initial Calculations in Excel:**
   - Utilized Excel to calculate Gross Revenue, Total Tax, and Net Revenue from the 'Tailwind-Traders-Sales.xlsx' file.
   
2. **Data Preparation and Transformation in Power BI:**
   - Loaded data from 'Tailwind-Traders-Sales.xlsx', 'Purchases.xlsx', and 'Countries.xlsx'.
   - Ensured data consistency by optimizing data types and created an Exchange Data table via Python Script (`StringIO`, `pd.read_csv()`).
   - Created a **Sales in USD** table and a **CalendarTable** table using DAX.
   - The **Yearly Profit Margin** column was added to the **Sales in USD** table, alongside three key measures: 
     - **Quarterly Profit Margin** using `DATESQTD()`
     - **YTD Profit** using `TOTALYTD()`
     - **Median Sales** using `MEDIAN()`

3. **Data Modeling and DAX:**
   - Established relationships between the following tables in the model view:
     - **Countries** and **Exchange Data**
     - **Sales** and **Countries**
     - **Purchases** and **Sales**
     - **CalendarTable** and **Purchases**
     - **Sales in USD** and **Sales**

4. **Visualization Design:**
   - Designed three main dashboard pages: Sales Overview, Purchases Overview, and Profit Overview, featuring bar charts, map visuals, line charts, and KPIs.
   - Synchronized slicers for country-level filtering across pages.
   - Implemented interactive elements, including page navigation buttons and forecast analysis for enhanced decision-making capabilities.

5. **Power BI Service:**
   - Published the final report to Power BI Service and created **'Tailwind Traders Executive Dashboard'**.
   - Pinned visuals to create a dedicated executive dashboard.
   - Configured the mobile view for optimized access on all devices.
   - Set up an alert on the KPI visual for Gross Revenue, ensuring real-time monitoring of critical business metrics.

[**View the Live Dashboard on Power BI Service**](https://app.powerbi.com/links/HjlOYqOyhQ?ctid=c15b6c02-fcb2-4974-a518-d2dce9300b4b&pbi_source=linkShare)

## Key Insights

- **Sales Analysis:** The Sales Overview highlights key revenue-generating countries and products, helping Tailwind Traders prioritize areas with the highest sales.
- **Purchasing Behavior:** By examining supplier and product category trends, the dashboard uncovers areas for optimization in procurement and supplier management.
- **Profit Margins:** Profit Overview tracks quarterly and yearly profit margins, providing clarity on financial health and long-term profitability.

## Data and Files Included
- **Tailwind-Traders-Sales.xlsx** - Raw sales data used for initial calculations.
- **Purchases.xlsx** - Purchase data including supplier and product information.
- **Countries.xlsx** - Country details for geographical analysis.
- **Tailwind Traders Report.pbix** - The final Power BI report with all transformations, DAX measures, and visualizations.

## Snapshots of Dashboard
![Sales Overview](https://github.com/user-attachments/assets/7296e2cb-c4b6-415f-bf95-991d9e53c755)
![Purchase Overview](https://github.com/user-attachments/assets/73c7875f-5168-43d4-839b-610318af29d1)
![Profit Overview](https://github.com/user-attachments/assets/1d2ee43d-46fb-419e-8e07-5290907cf0e4)



## Conclusion
This Power BI project offers comprehensive insights into the performance of Tailwind Traders, highlighting critical KPIs that inform decision-making at the executive level. The dashboard provides a scalable solution for monitoring sales, purchases, and profitability across regions. Future enhancements could involve integrating predictive analytics, customer segmentation analysis, and real-time sales forecasting to further support strategic decision-making.
