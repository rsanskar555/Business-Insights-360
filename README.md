### 📌 Overview
A multi-functional Power BI dashboard that gives AtliQ Hardware a 360° view of its global business performance — spanning Finance, Sales, Marketing, Supply Chain, and Executive reporting. This was AtliQ's first foray into data-driven decision-making using Power BI, replacing ad-hoc Excel analyses that previously led to costly misjudgments (e.g., a failed store launch in the US).

### 🛠️ Tech Stack
- **Power BI Desktop** – Dashboard design and visualization
- **SQL (MySQL)** – Source database for transactional data
- **Excel / CSV** – Secondary data source
- **DAX** – Calculated columns, measures, KPIs
- **DAX Studio** – Report performance optimization
- **Power Query (M Language)** – Data transformation and date table creation

### 🗂️ Data Model
Built using the **Snowflake schema** methodology with the following key tables:

**Dimension Tables**
- `dim_customer` – 75 customers across 27 markets, 2 platforms (Brick & Mortar, E-Commerce), 3 channels
- `dim_market` – 27 markets, 7 sub-zones, 4 regions (APAC, EU, LATAM, NA)
- `dim_product` – 3 divisions (P&A, PC, N&S), 14 categories, multiple variants

**Fact Tables**
- `fact_sales_monthly` – Monthly actual sales quantities
- `fact_forecast_monthly` – Monthly demand forecasts for inventory optimization
- `freight_cost`, `gross_price`, `manufacturing_cost`, `pre_invoice_deductions`, `post_invoice_deductions`

### 📊 Dashboard Views

| View | Purpose |
|------|---------|
| 🏠 Home | Navigation hub to all views |
| 💰 Finance View | P&L analysis, gross margin, net sales trends |
| 🛒 Sales View | Customer and product-level sales performance |
| 📣 Marketing View | Campaign ROI and segment performance |
| 🔗 Supply Chain View | Forecast accuracy, inventory risk |
| 🧭 Executive View | Top-level KPIs for leadership |
| 🛍️ Products | Product performance deep-dive |

### ✨ Key Highlights
- Pulled data from **2 heterogeneous sources** (MySQL database + Excel/CSV files) into a unified model.
- Optimized report performance using **DAX Studio**, achieving a **5% improvement** in load and query time.
- Used bookmarks, page navigation buttons, dynamic titles, KPI indicators, and conditional formatting for a polished UX.
- Implemented a custom date table using **M Language** and divide-safe DAX measures to prevent zero-division errors.

### 📈 Business Impact
- Enabled AtliQ Hardware to analyze sales trends across global markets and all departments in one platform.
- Projected to drive a **10% acceleration in revenue** by enabling faster, data-backed decisions.
- Estimated **20% reduction in data-related expenses** by replacing fragmented Excel reports with a single source of truth.

### 💡 Power BI Techniques Used
- Calculated columns and measures with DAX
- Bookmarks for toggling between visuals
- Dynamic titles based on applied filters
- KPI indicators and conditional formatting (icons + background color)
- Published to Power BI Service with personal gateway for auto-refresh
- Power BI App creation with workspace collaboration and access permissions
- Large file version control via **GitHub LFS**
