bash

cat /mnt/user-data/outputs/adventureworks-dashboard/README.md
Output

# 📊 AdventureWorks Sales & Business Intelligence Dashboard

An end-to-end Power BI project built to analyze sales, revenue, returns, and customer performance for **AdventureWorks**, a global manufacturer of cycling equipment and accessories.

## 🎯 Project Overview

As a Business Intelligence Analyst, the goal of this project was to help the management team:
- Track key business metrics (sales, revenue, profit, returns)
- Compare performance across regions and sales territories
- Analyze product-level and category-level sales trends
- Identify high-value customers and key purchasing segments

Raw data was provided as multiple CSV files covering transactions, returns, products, customers, and sales territories.

## 🛠️ Tools & Skills Used

- **Power BI Desktop** – data modeling & dashboard design
- **Power Query** – data connection, cleaning & transformation
- **DAX (Data Analysis Expressions)** – calculated columns & measures
- **Data Modeling** – star-schema relational model with fact/dimension tables
- **AI Visuals** – Decomposition Tree, Key Influencers, Q&A tooltips

## 🗂️ Data Model

Built a star-schema model connecting Sales Data and Returns Data (fact tables) to Territory, Calendar, Customer, and Product lookup tables (dimensions), with Product Subcategories and Categories as a snowflaked hierarchy.

## 🔄 Workflow

1. **Connect & Shape Data** – Imported raw CSV files, cleaned and transformed tables using Power Query
2. **Build Data Model** – Created relationships between fact tables (Sales, Returns) and dimension tables (Territory, Calendar, Customer, Product, Categories/Subcategories)
3. **DAX Measures** – Wrote calculated columns and measures for KPIs like Total Revenue, Total Profit, Return Rate, Revenue per Customer, Monthly trends vs. prior month
4. **Dashboard Design** – Built a 7-page interactive report with KPI cards, trend charts, maps, decomposition trees, and AI-powered insights

## 📈 Report Pages

| Page | What it shows |
|---|---|
| **Exec Dashboard** | Company-wide KPIs (Revenue, Profit, Orders, Return Rate), revenue trend line, orders by category, top 10 products by orders/revenue/return %, most ordered & most returned product types |
| **Map** | Geographic breakdown of sales across Europe, North America, and Pacific regions |
| **Product Detail** | Drill-down view for a selected product — monthly orders/revenue/profit vs. target, profit trending, adjustable price simulation, auto-generated report summary |
| **Customer Detail** | Unique customers, revenue per customer, top 100 customers table, orders by income level & occupation, top customer by revenue |
| **Category Tooltip** | Weekly orders trend with revenue, profit, orders, and return KPIs |
| **Decomposition Tree** | Breaks down Total Orders by Category → Subcategory → Product for root-cause exploration |
| **Key Influencers** | AI-powered analysis of what drives metrics like Average Retail Price, plus customer segmentation by homeownership |

## 📈 Dashboard Preview

![Exec Dashboard](screenshots/1.Exec%20Dashboard.png)

| Map View | Product Detail |
|---|---|
| ![Map](screenshots/2.Map.png) | ![Product Detail](screenshots/3.Product%20Detail.png) |

| Customer Detail | Category Tooltip |
|---|---|
| ![Customer Detail](screenshots/4.Customer%20Detail.png) | ![Category Tooltip](screenshots/5.Category%20Tooltip.png) |

| Decomposition Tree | Key Influencers |
|---|---|
| ![Decomposition Tree](screenshots/6.Decomposition%20Tree.png) | ![Key Influencers](screenshots/7.Key%20Influencers.png) |

## 📁 Repository Structure

```
PowerBI---Projects/
├── adventureworks-dashboard/
│   ├── Adventure_Works.pbix     # Power BI project file
│   └── README.md                # this file
├── screenshots/                 # dashboard screenshots
│   ├── 1.Exec Dashboard.png
│   ├── 2.Map.png
│   ├── 3.Product Detail.png
│   ├── 4.Customer Detail.png
│   ├── 5.Category Tooltip.png
│   ├── 6.Decomposition Tree.png
│   └── 7.Key Influencers.png
└── README.md                    # repo overview
```

## 🚀 How to View

1. Download `dashboard.pbix`
2. Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only)
3. Explore the interactive report pages

## 📌 Key Insights

- Generated **$25M in total revenue** and **$10M in profit** across ~25K orders, with a healthy **2.2% return rate**
- **Accessories** is the top-selling category by orders (~17K), followed by Bikes (~13.9K) and Clothing (~7K)
- **Tires and Tubes** is the leading subcategory within Accessories, with Patch Kits and Mountain Tire Tubes as top sellers
- Revenue shows strong upward momentum from 2021 into 2022, with a sharp growth inflection in early 2022
- **17.4K unique customers** generated an average revenue per customer of ~$1,430
- Sales are concentrated in North America and Europe (US, Canada, UK, Germany, France), with a smaller presence in the Pacific (Australia)
- Key Influencers analysis shows Average Retail Price rises strongly with Product Cost, and customer segments with higher homeownership rates show distinct purchasing patterns

## 📚 Acknowledgment

This project was built by following a guided Power BI course (Maven Analytics – *Up & Running with Power BI Desktop*, instructed by Chris Dutton & Aaron Parry) as a hands-on way to practice data modeling, DAX, and dashboard design. The dataset (AdventureWorks) is a Microsoft-provided sample dataset used for training purposes.

While the project structure follows the course, all data transformations, DAX measures, and the final dashboard were built and configured independently as part of the learning process.

---
⭐ If you found this project useful, feel free to star the repo!
