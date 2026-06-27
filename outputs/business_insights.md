# Task 3

# Business Insights – Calculated Fields

## Overview

The following calculated fields were developed within Tableau to facilitate executive analysis and data-driven decision-making.

| Calculated Field | Tableau Formula | Business Purpose |
| :--- | :--- | :--- |
| **Profit Margin** | `SUM([Profit]) / SUM([Sales])` | Indicates the percentage of revenue captured as profit; higher values reflect stronger operational efficiency. |
| **Cost** | `SUM([Sales]) - SUM([Profit])` | Derives the expenditure required to generate sales, allowing for refined profitability assessments. |
| **Average Order Value** | `SUM([Sales]) / COUNTD([Order ID])` | Tracks the average revenue per order to gauge shifting customer purchasing power. |
| **Return Rate** | `SUM([Return Flag]) / COUNTD([Order ID])` | Highlights the proportion of returned orders relative to total unique transactions. |
| **Shipping Delay Bucket** | `IF [Delivery Days] <= 2 THEN "Fast Delivery" ELSEIF [Delivery Days] <= 5 THEN "Standard Delivery" ELSE "Delayed Delivery" END` | Segments logistics performance into actionable categories for identifying shipping bottlenecks. |

---

## Business Interpretation

### Profit Margin
This metric quantifies how effectively the organization translates sales into bottom-line profit. Elevated margins signal robust financial health and disciplined cost control.

### Cost
By isolating the expenses tied to specific sales, this metric serves as a key indicator of operational efficiency.

### Average Order Value
This provides visibility into customer spending habits, acting as a foundation for pricing adjustments and marketing outreach.

### Return Rate
Elevated return rates serve as a diagnostic trigger for potential product quality, fulfillment, or customer expectation discrepancies.

### Shipping Delay Bucket
Categorizing deliveries into **Fast**, **Standard**, and **Delayed** workflows enables targeted logistics monitoring and continuous improvement of delivery timelines.

---

## Summary
These calculated fields form the backbone of the executive dashboard, enabling granular analysis of profitability, operational costs, customer behavior, and fulfillment quality. They collectively empower leadership to make informed, strategic decisions.

---

# Task 8

# Business Insights

## Overview
The executive dashboard provides a comprehensive view of sales performance, profitability, customer demographics, shipping efficiency, and return trends. The following analysis is derived directly from the underlying dataset and visual metrics.

---

# Insight 1 – Sales Trend

### Observation
Sales performance exhibits seasonal trends throughout the year, with notable surges in **February** and **October**, and a comparative trough in **April**.

### Data Evidence
* February Sales: **₹20.34 Million**
* October Sales: **₹19.84 Million**
* April Sales: **₹15.21 Million**

### Business Interpretation
The revenue cycle is subject to seasonal demand fluctuations.

### Recommended Action
Optimize inventory levels and align promotional cycles with identified peak demand months, while conducting a root-cause analysis for the April decline.

---

# Insight 2 – Regional Performance

### Observation
The **South** region currently serves as the leading driver of both sales volume and total profit.

### Data Evidence
* South Sales: **₹64.69 Million**
* South Profit: **₹9.99 Million**
* Performance metrics indicate that the South region consistently outperforms the North, East, and West territories.

### Business Interpretation
The South region represents the organization’s most vital market and a model for operational success.

### Recommended Action
Analyze and codify the successful sales tactics employed in the South to facilitate knowledge transfer and adoption in underperforming regions.

---

# Insight 3 – Category and Sub-Category Profitability

### Observation
The **Technology** category stands out as the primary engine for profitability.

### Data Evidence
* Technology Profit: **₹28.04 Million**
* Furniture Profit: **₹3.56 Million**
* Office Supplies Profit: **₹1.71 Million**
* **Copiers** contribute the highest profit at the sub-category level, reaching approximately **₹7.31 Million**.

### Business Interpretation
Technology products are the primary driver of corporate earnings.

### Recommended Action
Scale investments in the Technology sector while re-evaluating the pricing and product mix for the Furniture and Office Supplies divisions to bolster their margins.

---

# Insight 4 – Customer Segment Behavior

### Observation
The **Home Office** segment leads as the most significant contributor to total sales volume.

### Data Evidence
* Home Office Sales: **₹74.50 Million**
* Consumer Sales: **₹71.89 Million**
* Corporate Sales: **₹70.63 Million**

### Business Interpretation
Home Office customers represent the most valuable revenue stream.

### Recommended Action
Implement tailored loyalty initiatives for Home Office clients while executing growth strategies to capture more market share within the Corporate and Consumer segments.

---

# Insight 5 – Discount Impact

### Observation
Profitability exhibits a clear inverse relationship with discount levels; aggressive discounting is eroding the bottom line.

### Data Evidence
* 0% Discount Average Profit: **₹13,203**
* 25% Discount Average Profit: **₹3,113**
* 35% Discount Average Profit: **−₹1,601**

### Business Interpretation
Excessive price reductions are a major contributor to reduced net profitability.

### Recommended Action
Restrict high-discount campaigns unless they are proven to drive significant volume that offsets the margin loss.

---

# Insight 6 – Shipping Performance

### Observation
Fulfillment speed is highly correlated with the chosen shipping method.

### Data Evidence
Average Delivery Days:
* Same Day: **0.40 Days**
* First Class: **1.77 Days**
* Second Class: **2.68 Days**
* Standard Class: **4.71 Days**

### Business Interpretation
Variability in shipping times is largely dictated by the selected service level.

### Recommended Action
Focus operational improvements on Standard Class logistics to reduce lead times and nudge urgent buyers toward premium shipping options.

---

# Insight 7 – Return Pattern

### Observation
The **Furniture** category exhibits the highest frequency of product returns.

### Data Evidence
Return Rates:
* Furniture: **7.67%**
* Office Supplies: **3.65%**
* Technology: **3.03%**
* The **East** region leads with the highest return rate at **4.91%**.

### Business Interpretation
Recurring returns in the Furniture category suggest potential issues with product durability, expectation alignment, or shipping damage.

### Recommended Action
Perform a deep-dive analysis into Furniture returns to identify specific quality or shipping failure points, then implement corrective measures.

---

# Insight 8 – Business Risk and Opportunity

### Observation
Profitability can be scaled by balancing high-performing regions and margins while mitigating the impact of returns and deep discounts.

### Data Evidence
* Overall Sales: **₹217.02 Million**
* Overall Profit: **₹33.31 Million**
* Profit Margin: **15.35%**

### Business Interpretation
While the company is fundamentally sound, profit optimization depends on reinforcing high-margin product lines and controlling operational "leaks" like returns and deep discounting.

### Recommended Action
Focus on expanding the Technology footprint, optimizing regional discounting policies, and launching initiatives to decrease Furniture return rates.

---

# Executive Summary

The business demonstrates robust health with **₹217.02 Million** in total sales and a **15.35%** profit margin. Primary profitability is anchored by Technology products and the South region. Conversely, Furniture returns and aggressive discounting are identified as the primary operational risks. Strategic prioritization of successful product lines, coupled with disciplined regional strategies and return-mitigation initiatives, will position the company for sustainable growth.
