**Nike Sales Dashboard**

This project presents a Power BI Dashboard visualizing Nike sales data, including product performance, regional profits, and sales trends over time.

Project Structure

- Dataset: Sourced from Kaggle (Nike Sales Dataset).
    Kaggle: [Nike Sales Dataset](https://www.kaggle.com/datasets/nayakganesh007/nike-sales-uncleaned-dataset) (used for learning purposes)
- Tool Used: Power BI (with Power Query for cleaning and DAX for calculations).
- Main File: `.pbix` (Power BI file containing the dashboard).
- Image: Dashboard screenshot for reference.



**Data Cleaning (in Power Query)**

- Converted Size values i.e., Standardization (`L`, `M`, `XL`) to numeric (e.g., `L` = 8, `M` = 7, `XL` = 9).
- Replaced missing values in:
  - `Size` with `0`
  - `Order_Date` with a placeholder date `01/01/2025`
  - `Units_Sold`, `MRP` with `0`
- Ensured all column data types are consistent (e.g., decimal for `MRP`, whole number for `Units_Sold`, date for `Order_Date`).

DAX Measures Used:
- Sum of Profit = SUM(Sales[Profit])
- Sum of MRP = SUM(Sales[MRP])
- Sum of Units_Sold = SUM(Sales[Units_Sold])
- Count Of Product = COUNT(Sales[Product])
- Average MRP = AVERAGE(Sales[MRP])



**Visuals:**

- Bar chart: Units Sold by Gender
- Line chart: Revenue & Profit by Year
- Pie chart: Profit by Region
- Donut chart: Revenue by Sales Channel
- Column chart: Units Sold by Product Line



- KPI Cards for:

  - Total Profit

  - Total MRP

  - Total Units Sold

  - Product Count

  - Average MRP




**Slicers:**

- Region selector (handles city name inconsistencies like "Hyd", "Hyderabad", "hyd")

- Date range filter using Order_Date

**This dashboard is for educational and portfolio purposes.**

Created by Anurag Phalke (
anuragphalke777@gmail.com)
