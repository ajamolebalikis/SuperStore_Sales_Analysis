# SuperStore_Sales_Analysis

# 🏬 Super Store Sales Analysis (Power BI Project)

## 🪄 Introduction
This project analyzes the **Super Store dataset** using **Power BI** to uncover key insights into sales performance, customer behavior, product profitability, and regional trends.  
The dataset contains information across multiple tables — **Orders, Customers, Locations, States, Products, and Product Pricing Tiers**. 
The goal of this project is to **understand business performance** through metrics such as total sales, profit, customer growth, product performance, and regional contribution.  
By applying **data modeling, DAX measures, and visual storytelling**, this report delivers a clear, data-driven overview of operational strengths, weaknesses, and opportunities for improvement.
---

## ⚠️ Disclaimer
This dataset was used **strictly for learning and demonstration purposes**.  
It does **not represent any real company's data**, customers, or transactions.  
All names, figures, and locations are fictional or anonymized.

---

## 📑 Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Data Preparation](#data-preparation)
4. [Data Modeling](#data-modeling)
5. [DAX Measures](#dax-measures)
6. [Visuals and Dashboard Pages](#visuals-and-dashboard-pages)
7. [Key Insights](#key-insights)
8. [Recommendations](#recommendations)
9. [Tools Used](#tools-used)
10. [Conclusion](#conclusion)
11. [Author](#author)

---

## 🧭 Project Overview
The Super Store Sales Analysis project provides a detailed examination of a retail store’s operations over a four-year period (2014–2017).  

It aims to identify:
- Trends in **sales and profit performance**  
- **Customer and regional behaviors** influencing sales  
- **Top and underperforming products** by category and subcategory  
- Year-over-year (**YoY**) and same period last year (**SPLY**) performance metrics  

The project demonstrates how data modeling, DAX calculations, and visualization storytelling can be used to uncover actionable insights and improve overall business performance.

---

## 🗂️ Dataset Description
The dataset consists of six tables:
1. **Orders** – Contains details of all customer orders.
2. **Customers** – Information about each customer.
3. **Products** – Product details such as name and category.
4. **Product Pricing Tiers** – Defines price categories for each product.
5. **States** – Contains information about states within regions.
6. **Locations** – Includes regional and city-level location data.

The dataset spans from **2014 to 2017**.

---

## 🧹 Data Preparation
Data cleaning and transformation were carried out in **Power Query**:
- Removed **duplicates**  
- Promoted **column headers**  
- Ensured **data type consistency**  
- Removed **null and irrelevant fields**  
- Created a **Date Table** using DAX for time intelligence analysis  

After transformations, the dataset was **loaded into Power BI** using the *Close & Apply* function.

---

## 🔗 Data Modeling
Relationships were created among the tables to ensure efficient data interaction:
- The **Products** table was connected to the **Product Pricing Tier** table.
- The **Orders** table was linked with **Customers**, **States**, and **Products**.
- The **Date Table** was connected to the **Orders** table via *Order Date*.

The model was built as a **star schema**, ensuring optimized reporting performance.

---

## 📊 DAX Measures
### **Base Measures**
- Total Sales  
- Total Profit  
- Total Orders  
- Total Quantity  
- Total Customers  
- Profit Margin  
- Average Discount  
- Loss Percentage (%)  
- Loss Count  

### **SPLY (Same Period Last Year) Measures**
- SPLY Customers  
- SPLY Discount  
- SPLY Orders  
- SPLY Profit  
- SPLY Profit Margin  
- SPLY Quantity  
- SPLY Sales  

### **YoY (Year-over-Year) Growth Measures**
- YoY Customers %  
- YoY Discount %  
- YoY Orders %  
- YoY Profit %  
- YoY Profit Margin %  
- YoY Quantity %  
- YoY Sales %  

### **SVG Sparklines**
Created using the **SVG method** in Power BI for mini area charts representing trends for:
- Customers  
- Discount  
- Orders  
- Profit  
- Profit Margin  
- Quantity  
- Sales  

---

## 📈 Visuals and Dashboard Pages
The dashboard consists of **four interactive pages** with slicers for **Region**, **Category**, and **Year**.

### **1️⃣ Sales Overview Page**
- **KPI Cards**
  - Total Sales: **$173K** (YoY +1%)  
  - Total Profit: **$18K** (YoY +1%)  
  - Total Orders: **793** (YoY +1%)  
  - Profit Margin: **12%** (YoY +2%)  
- **Sales by State:** California, New York, and Texas ranked highest; South Dakota and Iowa lowest.  
- **Sales vs Profit by Month:** May recorded the highest sales; October and February were the lowest.  
- **Sales by Customer Segment:** Consumers lead, followed by Corporate and Home Office.  
- **Sales by Category:** Furniture ranked highest, followed by Technology and Office Supplies.

---

### **2️⃣ Product Performance Page**
- **Top 10 Subcategories:** Phones, Chairs, and Tables lead in sales; Machines and Appliances lag.  
- **Loss Count by Subcategory:** Binders, Tables, and Chairs have the most loss; Fasteners and Supplies the least.  
- **Category-Level Analysis:**
  - *Furniture* tops in sales, followed by *Technology* and *Office Supplies*.  
  - *Office Supplies* leads in quantity sold.  
- **Sample Insights:**
  - *Binders:* 123 customers, YoY sales +1%, profit margin −20%  
  - *Chairs:* 47 customers, YoY sales +2%, profit margin +8%  
  - *Envelopes:* 21 customers, YoY sales +16%, profit margin +41%  
  - *Phones:* 63 customers, YoY sales +3%, profit margin +16%

---

### **3️⃣ Customer Performance Page**
- **Top 10 Customers by Sales:** Christopher Conant, John Murray, Luke Weiss, Bill Donatelli, Luke Foster.  
- **Customer by Category:** Office Supplies highest.  
- **Customer by Ship Mode:** Standard Class most common, followed by Second Class.  
- **Customer by Region:** West region has the largest customer base; South the least.  
- **Customer by Month:** March–June recorded the highest activity; October and February lowest.

---

### **4️⃣ Regional Performance Page**
- **Total Orders by State:** California, Texas, New York, and Illinois lead.  
- **Total Sales by Region:** East region ranks highest, followed by West and South.  
- **Total Profit by Region:** South and East regions are most profitable; Central region least.  
- **Top Performing States by Profit:** New York, Virginia, California, Kentucky, Washington, Illinois.

---

## 💡 Key Insights
- California, New York, and Texas are the **top-performing states** by both sales and profit.  
- *Furniture* and *Technology* categories dominate sales.  
- *Binders* and *Tables* recorded the **highest loss counts**.  
- *Consumer segment* generates the highest sales volume.  
- Profit margin stands at **12%**, with **positive 2% YoY growth**.  
- Sales seasonality shows strong months between **March and June**.  
- The **East region** consistently outperforms other regions in sales and profit.

---

## 🧠 Recommendations
1. Increase focus on **high-performing regions** (East & South) with targeted promotions.  
2. Re-evaluate pricing and marketing for **loss-leading products** like binders and tables.  
3. Encourage **corporate and home office segments** with loyalty incentives.  
4. Strengthen inventory for **high-demand months** (March–June).  
5. Improve **profitability** by optimizing discount policies.  
6. Expand customer acquisition in **underperforming regions** (Central & South).  

---

## 🧰 Tools Used
- **Power BI Desktop** – Data modeling, DAX, and visualization  
- **Power Query Editor** – Data cleaning and transformation  
- **DAX (Data Analysis Expressions)** – Measures, KPIs, and time intelligence  
- **SVG in Power BI** – Custom sparklines visualization  

---

## 🏁 Conclusion
The **Super Store Sales Analysis Dashboard** provides a comprehensive understanding of how different factors—products, customers, and regions—impact business performance.  
Through time intelligence (YoY and SPLY), it uncovers year-over-year growth and seasonal trends, supporting strategic decision-making.  

Overall, the dashboard serves as a valuable analytical tool for tracking performance, identifying improvement areas, and driving profit growth.

---

## 👩‍💻 Author
**Name:** Balikis Ajamole  
**Role:** Data Analyst  
**Tools:** Power BI | DAX | Power Query | Data Modeling  
**Contact:** [ajamolefolake@gmail.com]  

---
