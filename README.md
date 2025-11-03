# 🛒 E-Commerce Sales Analysis Dashboard (Excel)

An interactive **Excel dashboard** designed to analyze and visualize key e-commerce performance metrics such as sales, profit, orders, and product categories.  
This project leverages Excel’s data analytics capabilities — including pivot tables, charts, and slicers — to turn raw sales data into actionable business insights.

---

## 📊 Dashboard Overview

![E-Commerce Sales Dashboard](https://github.com/ths887/E-Commerce-Sales-Analysis-Dashboard-Excel-/blob/main/Ecommerce%20Sales%20Analysis%20Dashboard-%20Image.png?raw=true)

---

## ✅ Key Insights

- 💰 **Sales & Profit Overview** — Displays total sales, profit, and year-over-year growth  
- 📈 **Sales and Profit Analysis** — Compares monthly sales and profit trends  
- 🏷️ **Category Performance** — Highlights category- and subcategory-wise revenue share  
- 🗺️ **Sales by State** — Visualized through an interactive U.S. map chart  
- ⚙️ **Interactive Filters** — Filter data by year, region, and segment for deeper insights  

---

## 🎯 Business Impact

This dashboard helps business analysts and decision-makers to:

- Monitor key sales and profitability trends  
- Identify top-performing product categories  
- Understand regional sales distribution  
- Enhance strategic planning with data-driven insights  

---

## 🧰 Tools & Techniques Used

| Tool | Purpose |
|------|----------|
| **Microsoft Excel** | Dashboard creation & visualization |
| **Pivot Tables** | Summarize and analyze key sales metrics |
| **Charts (Column, Bar, Pie, Map)** | Display trends and comparisons |
| **Slicers & Filters** | Enable interactive data exploration |
| **Conditional Formatting** | Highlight year-over-year growth |
| **DAX (Data Analysis Expressions)** | Custom KPIs & calculated measures (e.g., YoY Growth, Profit Margin) |

---


## 🧮 Example DAX Measures Used

Total Sales = SUM(Sales[SalesAmount])

Total Profit = SUM(Sales[Profit])

YoY Sales Growth (%) =
VAR CurrentYearSales = [Total Sales]
VAR PreviousYearSales =
    CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
RETURN
DIVIDE(CurrentYearSales - PreviousYearSales, PreviousYearSales, 0)

---

## 📂 Project Structure

