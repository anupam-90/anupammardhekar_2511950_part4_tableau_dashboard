# Retail Sales & Profitability Executive Dashboard

## 1. Business Problem Summary

The leadership team needed a centralized way to track retail performance. This project transforms raw transaction data into an interactive Tableau dashboard, allowing stakeholders to monitor key metrics, identify operational risks, and find growth opportunities through data-driven insights.

---

## 2. Dataset Description

The analysis is based on order-level retail data covering:
* **Temporal:** Order and shipping dates.
* **Geographic:** Region, State, and City.
* **Customer:** Customer ID and Segment.
* **Product:** Category, Sub-Category, and Product Name.
* **Financials:** Sales, Profit, Quantity, and Discount.
* **Operations:** Ship Mode, Delivery Duration, and Return Status.

---

## 3. Tableau Workbook Description

The workbook acts as a comprehensive reporting interface, featuring an executive dashboard supported by specific analytical worksheets:

* **Core Visuals:** Sales trends, regional performance, category profitability, and customer segments.
* **Operational Visuals:** Shipping efficiency, the impact of discounts on profit, and return analysis.
* **KPIs:** High-level summary of Total Sales, Total Profit, and Profit Margin.

---

## 4. Calculated Fields Created

To enable deeper analysis, the following fields were developed:

| Calculated Field | Formula | Purpose |
| :--- | :--- | :--- |
| **Profit Margin** | `SUM([Profit]) / SUM([Sales])` | Measures overall profitability. |
| **Cost** | `SUM([Sales]) - SUM([Profit])` | Estimates operational cost. |
| **Average Order Value** | `SUM([Sales]) / COUNTD([Order ID])` | Tracks revenue per order. |
| **Return Rate** | `SUM([Return Flag]) / COUNTD([Order ID])` | Tracks percentage of returned orders. |
| **Shipping Delay Bucket** | `IF [Delivery Days] <=2 THEN "Fast" ...` | Categorizes shipping speed. |

---

## 5. Dashboard Components

* **KPI Cards:** Real-time totals for Sales, Profit, and Margin.
* **Visualizations:** Trends, regional breakdowns, and comparative analysis (Discount vs. Profit, Return Analysis).

---

## 6. Filters and Interactions

Users can perform exploratory analysis using interactive filters for **Region, State, Category, Customer Segment, Ship Mode,** and **Order Date.** A "Filter Action" is enabled, allowing users to click a specific region to instantly update all related charts.

---

## 7. Key Business Insights

* **Performance:** Sales remain stable with seasonal peaks.
* **Top Performers:** The South region leads in revenue; Technology and Copiers are the most profitable categories.
* **Opportunities:** Higher discounts directly correlate with lower profits.
* **Operational Hurdles:** Furniture shows the highest return rates, and Standard shipping consistently has the longest delays.

---

## 8. Dashboard Story Summary

This dashboard moves beyond isolated charts to provide a holistic business view. It guides the user from high-level financial KPIs down to specific operational issues like shipping delays and returns, providing a clear roadmap for improving profitability.

---

## 9. Assumptions and Limitations

* **Assumptions:** Data is standardized (currency, date formats), unique order IDs, and accurate return flags.
* **Limitations:** The scope is limited to historical data; it does not include predictive forecasting, inventory levels, or external market trends.

---

## 10. Screenshots Included

* `full_dashboard.png`
* `sales_trend_view.png`
* `regional_performance_view.png`
* `category_profitability_view.png`
* `filter_interaction_view.png`

---

## Project Structure

```text
Retail_Tableau_Project/
├── dashboard_sales_data.xlsx
├── tableau/
│   └── executive_dashboard.twbx
├── outputs/
│   ├── business_insights.md
│   └── dashboard_story.md
├── screenshots/
└── README.md
