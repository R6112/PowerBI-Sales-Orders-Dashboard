![Screenshot 2025-01-23 152156](https://github.com/user-attachments/assets/52b2dae1-a8b2-4efd-86e7-41e6c2eaac06)

![Screenshot 2025-01-23 152115](https://github.com/user-attachments/assets/a7d2dac0-37c6-4af7-88ed-5b6a216c0dc3)
![Screenshot 2025-01-23 152051](https://github.com/user-attachments/assets/12b216c5-b205-47fd-8baf-5bb92c51d8a3)

![Screenshot 2025-01-23 151846](https://github.com/user-attachments/assets/ee1303c7-3b29-4f6b-83ad-e0a2b052a084)
# PowerBI-Sales-Orders-Dashboard

## Overview
This repository contains a Power BI dashboard that visualizes sales order data. The dashboard uses KPIs and various visualizations, including cards and a waterfall chart, to present key metrics such as sales amounts, marketing amounts, and team performance.

## Key Visualizations and Metrics
- **Cards:**
  - **Total Sales Amount:** 1.04M (Sum of Sales Amount).
  - **Average Sales Amount:** 64.75K (Average Sales Amount).
  - **Sales Order Count:** 16 (Total Count of Sales IDs).

- **Waterfall Chart:** 
  - Displays the **Sum of Marketing Amount** and **Sum of Sales Amount** by month and sales team.
  - Provides insights into the month-over-month and team-level breakdown of sales and marketing efforts.

- **Multi-row Card:**
  - Displays **Sum of Sales Amount** for different months, allowing for easy comparison across time periods.

## DAX Calculations
Key DAX queries used in the dashboard:

- **Total Sales Amount:**
  ```DAX
  TotalSalesAmount = SUM('SalesOrders'[SalesAmount])
  ```

- **Average Sales Amount:**
  ```DAX
  AverageSalesAmount = AVERAGE('SalesOrders'[SalesAmount])
  ```

- **Sales Order Count:**
  ```DAX
  SalesOrderCount = COUNTROWS('SalesOrders')
  ```

- **Marketing Amount:**
  ```DAX
  MarketingAmount = SUM('SalesOrders'[MarketingAmount])
  ```

