# 📊 Business Performance Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

<br/>

[![🚀 Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-View%20Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://your-live-demo-link-here)

> **👆 Click above to view the interactive dashboard live on Power BI Service**

---
<img width="1438" height="804" alt="Screenshot 2026-05-19 142904" src="https://github.com/user-attachments/assets/6ee343ae-3524-4d97-a601-101dddf07c5f" />

<img width="1441" height="811" alt="Screenshot 2026-05-19 142928" src="https://github.com/user-attachments/assets/02efe17b-1e27-4166-912c-0e93c8622895" />

<img width="1451" height="819" alt="Screenshot 2026-05-19 142954" src="https://github.com/user-attachments/assets/7d0c5575-b579-423f-a52d-d7f0fa7228f1" />

<img width="1438" height="810" alt="Screenshot 2026-05-19 143026" src="https://github.com/user-attachments/assets/57ba713c-02ec-44e4-a7ba-5cd370c18c95" />

> A multi-page interactive Power BI dashboard providing a 360° view of business performance — from executive KPIs to regional store analysis.

---

## 📁 Dashboard Pages

| Page | Title | Focus Area |
|------|-------|------------|
| 1 | **Executive Overview** | High-level KPIs, revenue trends, category & country breakdown |
| 2 | **Sales & Product Analytics** | Product performance, brand revenue, profit by subcategory |
| 3 | **Customer Insights** | Customer behavior, retention, spend by age/country/gender |
| 4 | **Regional & Store Analysis** | Store-level revenue, store size & age analysis |

---

## 🔢 Key Metrics at a Glance

### Executive Overview
| Metric | Value |
|--------|-------|
| Total Revenue | **$55.76M** |
| Total Customers | **15,266** |
| Total Profit | **$32.66M** |
| Total Orders | **26,326** |

### Sales & Product Analytics
| Metric | Value |
|--------|-------|
| Total Quantity Sold | **26,326** |
| Avg Order Value | **$2.12K** |
| Top Product Revenue | **$505.45K** |
| Best Selling Product | **Adventure Works Desktop PC2.30 MD230 Black** |

### Customer Insights
| Metric | Value |
|--------|-------|
| Total Customers | **15,266** |
| Repeated Customers | **7,272** |
| Customer Retention Rate | **2.10** |
| Avg Customer Spend | **$3.65K** |
| High Value Customers | **3,932** |

### Regional & Store Analysis
| Metric | Value |
|--------|-------|
| Total Stores | **67** |
| Revenue Per Store | **$832.17K** |
| Revenue Per Sq. Meter | **$602.47** |
| Highest Revenue Country | **United States** |

---

## 📊 Visualizations Included

### Page 1 — Executive Overview
- 📈 **Line Chart** — Total Revenue by Month Name (Jan–Dec trend)
- 🍩 **Donut Chart** — Total Revenue by Category
- 📊 **Bar Chart** — Total Revenue by Country (Top 8)
- 📊 **Bar Chart** — Total Revenue by Product Name (Top 5)
- 📊 **Bar Chart** — Total Revenue by Gender (Male vs Female)

### Page 2 — Sales & Product Analytics
- 📊 **Horizontal Bar Chart** — Total Revenue by Category
- 📊 **Column Chart** — Total Revenue by Brand
- 🗺️ **Treemap** — Total Profit by Subcategory

### Page 3 — Customer Insights
- 🥧 **Pie Chart** — Total Customers by Gender
- 📊 **Column Chart** — Total Revenue by Age Group
- 📋 **Table** — Customer-level Revenue, Orders, Profit
- 📊 **Bar Chart** — Total Customers by Country

### Page 4 — Regional & Store Analysis
- 📊 **Histogram** — Total Revenue by Store Age
- 🍩 **Donut Chart** — Total Revenue by Store Size Group (Small / Medium / Large)
- 🗺️ **Treemap** — Total Revenue by Category (regional breakdown)

---

## 🎛️ Filters / Slicers

All pages share a consistent filter panel:

- 🌍 **Country** — Dropdown
- 🏷️ **Brand** — Dropdown
- 📅 **Month** — Dropdown
- 📅 **Quarter** — Dropdown
- 📅 **Year** — Button slicer (2016–2021)
- 🗂️ **Category** — Multi-select tile slicer

---

## 🏗️ Data Model Highlights

- **Fact Table**: Sales Transactions (Orders, Revenue, Profit, Quantity)
- **Dimension Tables**: Customers, Products, Stores, Date, Geography
- **Relationships**: Star schema with one-to-many relationships
- **Key DAX Measures**:
  - `Total Revenue = SUM(Sales[Revenue])`
  - `Total Profit = SUM(Sales[Profit])`
  - `Avg Order Value = DIVIDE([Total Revenue], [Total Orders])`
  - `Customer Retention Rate = DIVIDE([Repeated Customers], [Total Customers])`
  - `Revenue Per Store = DIVIDE([Total Revenue], DISTINCTCOUNT(Stores[StoreID]))`
  - `Revenue Per Sq. Meter = DIVIDE([Total Revenue], SUM(Stores[SquareMeters]))`
  - `High Value Customers = CALCULATE(DISTINCTCOUNT(Sales[CustomerID]), Sales[Revenue] > threshold)`

---

## 📂 Repository Structure

```
business-performance-dashboard/
│
├── BusinessPerformanceDashboard.pbix   # Main Power BI file
├── README.md                           # Project documentation
│
├── screenshots/
│   ├── executive_overview.png
│   ├── sales_product_analytics.png
│   ├── customer_insights.png
│   └── regional_store_analysis.png
│
└── data/
    └── sample_data.xlsx                # (Optional) Sample dataset
```

---

## 💡 Business Insights Derived

- 🇺🇸 **United States** dominates with **$30M** in revenue — 54% of total
- 💻 **Computers** is the top category at **$19.3M (34.62%)** of total revenue
- 🖥️ **Desktops** subcategory leads profit at **$5.63M**
- 📅 **February** peaks at **$7.6M**, while **March** dips to **$2.3M** — seasonal pattern observed
- 👨 **Male customers** slightly outspend female ($28M vs $27M)
- 🏪 **Large stores** generate the most revenue at **$22.02M (39.5%)**
- 👴 Age group **24–34** leads revenue at **$8.6M**
- 🔁 **47.6%** of customers are repeat buyers (7,272 out of 15,266)
- 🏆 **Adventure Works** brand dominates with **$11.8M** in revenue

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard design & publishing |
| **DAX** | Custom KPI measures & calculated columns |
| **Power Query (M)** | Data transformation & cleaning |
| **Excel / CSV** | Source data format |

---

## 🚀 How to Use

1. **Clone** this repository:
   ```bash
   git clone https://github.com/yourusername/business-performance-dashboard.git
   ```

2. **Open** `BusinessPerformanceDashboard.pbix` in **Power BI Desktop**

3. **Connect** your own data source or use the included sample data

4. **Refresh** the dataset via `Home → Refresh`

5. **Publish** to Power BI Service for sharing with stakeholders

---

## 📌 Prerequisites

- Power BI Desktop (latest version recommended)
- Windows OS (Power BI Desktop is Windows-only)
- Optional: Power BI Pro license for sharing via Service

---

## 🙋‍♂️ Author

**Hari** — Data Analyst | Power BI Developer

[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/yourusername)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-FF5722?style=flat&logo=google-chrome&logoColor=white)](https://yourportfolio.com)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

> ⭐ **If you found this useful, consider starring the repository!**

---

<div align="center">

### 🔗 Let's Connect on LinkedIn!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Hari-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/your-linkedin-username)

*Open to collaborations, feedback, and new opportunities!*

</div><img width="1438" height="804" alt="Screenshot 2026-05-19 142904" src="https://github.com/user-attachments/assets/44ffcf37-3ead-420c-a484-cef6cd6af219" />
