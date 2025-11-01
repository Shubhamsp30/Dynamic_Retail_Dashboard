# 🛍️ Dynamic Retail Dashboard  
### *Excel & Data Analytics Project by Shubham Vrushabhanath Patil*

---

## 📘 Project Overview  

This project presents a **Dynamic Retail Dashboard** built entirely in **Microsoft Excel**.  
The dashboard provides a comprehensive analysis of sales, profit, and operational efficiency for a retail business inspired by Walmart.  

By leveraging Excel’s analytical capabilities — including **Power Query**, **Pivot Tables**, **Slicers**, and **Dynamic Charts** — the dashboard helps in identifying patterns, visualizing performance, and drawing actionable insights for business growth.

---

## 🧠 Business Problem  

With growing customer demands and fierce market competition, Walmart aims to understand what drives its success and what areas need improvement.  

The company has collected detailed sales order data to identify:
- High-performing product categories and segments  
- Sales and profit trends across regions and years  
- Potential inefficiencies due to returns or high shipping costs  

---

## 🎯 Objective  

The main objectives of this project are:
- To gain insights into the **performance of the store**  
- To identify trends in **customer segments**, **product categories**, and **sales patterns**  
- To use **Excel analytics** for creating an **interactive dashboard**  
- To provide **data-driven recommendations** for operational improvement  

---

## 📊 Dataset Information  

**📁 Dataset Source:** [Excel Dataset on GitHub](https://raw.githubusercontent.com/starlordali4444/Acciojob-Excel/refs/heads/master/common_notes/data/excel_dataset.xlsx)

The dataset contains **three key tables**:

### 1️⃣ Orders Table
| Category | Sub-Category | Product Name | Sales | Quantity | Discount | Profit | Shipping Cost | Order Priority |
|-----------|--------------|---------------|--------|-----------|-----------|----------|----------------|----------------|

### 2️⃣ People Table
| Person | Region |
|---------|---------|

### 3️⃣ Returns Table
| Returned | Order ID | Market |
|-----------|-----------|--------|

---

## 📚 Data Dictionary  

| Field Name | Data Type | Description | KPI |
|-------------|------------|--------------|------|
| Order ID | Text | Unique identifier for each order | ✅ |
| Order Date | Date | Date when the order was placed | ❌ |
| Ship Date | Date | Date when the order was shipped | ❌ |
| Ship Mode | Text | Type of shipping selected (Same Day, Second Class, etc.) | ❌ |
| Customer ID | Text | Unique identifier for each customer | ✅ |
| Customer Name | Text | Full name of the customer | ❌ |
| Segment | Text | Customer segment (Consumer, Corporate, Home Office) | ❌ |
| City | Text | City of the customer | ❌ |
| State | Text | State/Province of the customer | ❌ |
| Country | Text | Country of the customer | ❌ |
| Postal Code | Whole Number | Postal code (null replaced with -1) | ❌ |
| Market | Text | Geographic market (US, APAC, EU, LATAM, etc.) | ❌ |
| Region | Text | Sub-region within the market | ❌ |
| Product ID | Text | Unique identifier for each product | ✅ |
| Category | Text | Product category | ❌ |
| Sub-Category | Text | Sub-category of the product | ❌ |
| Product Name | Text | Full name/description of the product | ❌ |
| Sales | Decimal | Sales revenue generated from the order | ✅ |
| Quantity | Whole Number | Quantity of items ordered | ✅ |
| Discount | Decimal | Discount applied to the order | ✅ |
| Profit | Decimal | Profit earned on the order | ✅ |
| Shipping Cost | Decimal | Cost of shipping the order | ✅ |
| Order Priority | Text | Priority of the order (Critical, Medium, etc.) | ❌ |

---

## 📈 Business KPIs  

The following **Key Performance Indicators (KPIs)** are used to summarize business performance:

1. **Total Sales**  
2. **Total Profit**  
3. **Total Quantity Sold**  
4. **Number of Orders**  
5. **Profit Margin (%)**

---

## 🧩 Dashboard Features  

| # | Analysis Type | Description |
|---|----------------|-------------|
| 1 | **Overall KPIs** | Snapshot of sales, profit, quantity, orders, and profit margin |
| 2 | **Sales & Profit Analysis** | Visual comparison of sales vs. profit |
| 3 | **Category-wise Profit** | Breakdown of profits by major product categories |
| 4 | **Segment-wise Sales Share %** | Contribution of each customer segment to total sales |
| 5 | **Sales by Country** | Geographic analysis of revenue performance |
| 6 | **Top 5 Sub-Categories** | Best-performing sub-categories by sales |
| 7 | **Bottom 5 Sub-Categories** | Lowest-performing sub-categories |
| 8 | **Yearly Sales Trend** | Year-over-year comparison of sales growth |

---

## ⚙️ Tools & Techniques Used  

- **Microsoft Excel**
  - Power Query (Data Cleaning & Transformation)
  - Pivot Tables for summarization
  - Slicers & Timelines for interactivity
  - Conditional Formatting for highlighting key metrics
  - Dynamic Charts for visualization

- **GitHub** for version control and dataset hosting

---

## 🧮 Workflow & Steps  

### Step 1️⃣: Data Loading  
- Imported the dataset from [GitHub Raw Link](https://raw.githubusercontent.com/starlordali4444/Acciojob-Excel/refs/heads/master/common_notes/data/excel_dataset.xlsx).  
- Verified column data types and structure in Excel.

### Step 2️⃣: Data Cleaning (Power Query)
- Removed duplicates and null values.  
- Replaced missing postal codes with `-1`.  
- Merged **Orders**, **People**, and **Returns** tables using relevant keys (Order ID, Region).  
- Ensured consistent formatting for text, numbers, and dates.

### Step 3️⃣: Data Modeling  
- Established relationships between the tables:  
  - `Orders[Region]` ↔ `People[Region]`  
  - `Orders[Order ID]` ↔ `Returns[Order ID]`
- Created calculated columns for **Profit Margin**, **Return Rate**, and **Average Shipping Cost**.

### Step 4️⃣: Dashboard Design  
- Created KPIs at the top (Sales, Profit, Orders, etc.).  
- Added slicers for **Year**, **Category**, **Segment**, and **Region**.  
- Used charts such as:
  - Bar chart (Category-wise Profit)
  - Pie/Donut (Segment-wise Share)
  - Line chart (Yearly Sales Trend)
  - Horizontal bar (Top/Bottom Sub-Categories)

### Step 5️⃣: Insights & Formatting  
- Added dynamic color coding for profit/loss zones.  
- Used data labels and number formatting for clarity.  
- Finalized dashboard layout with clean spacing and consistent design.

---

## 💡 Key Insights  

- **Technology** category generated the highest sales and profit.  
- **Furniture** category had strong sales but weaker profit margins.  
- **Corporate Segment** contributed the most to total revenue.  
- **LATAM market** showed the highest return rate.  
- **Discounts above 20%** significantly impacted profit negatively.  
- **Yearly trend** indicated consistent growth with seasonal peaks in Q4.

---

## 🚀 Future Enhancements  

- Integration with **Power BI** for live dashboards and advanced visuals.  
- Implementation of **forecasting models** using Excel’s built-in analytics tools.  
- Region-wise performance tracking using **geo-maps**.  
- Automated dataset refresh through Power Query connections.

---

## 👨‍💻 Author  

**Shubham Vrushabhanath Patil**  
📍 B.Tech – Electronics and Telecommunication Engineering  
💻 Data Analytics & Visualization Enthusiast  
📧 [GitHub Profile](https://github.com/Shubhamsp30)  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/shubhampatil30/)  

---

## 🖼️ Dashboard Preview  


> <img width="1241" height="720" alt="Screenshot 2025-11-01 180645" src="https://github.com/user-attachments/assets/c51b24ec-654d-44b4-abeb-90725e99e071" />


---

## ⭐ Contribute  

If you liked this project:
- ⭐ Star this repository  
- Fork it and share your insights  
- Connect with me on LinkedIn for collaboration  

---

## 📢 Tags  

#ExcelDashboard #DataAnalytics #PowerQuery #RetailAnalytics #EDA #WalmartCaseStudy #BusinessInsights #DataVisualization #ExcelProjects #GitHubPortfolio
