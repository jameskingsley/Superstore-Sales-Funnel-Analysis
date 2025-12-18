

# Superstore Sales Funnel Analysis
###### Overview

This project explores sales funnel analysis for a supermarket chain using the Sample Superstore dataset. The main goal is to understand how discounts impact order progression and profitability across product categories and geographical regions.

###### The analysis helps answer key business questions:
* Which product categories lose profitability under high discounts?
* Which regions sustain profit even when aggressive discounts are applied?
* How can discount strategies be tailored for maximum margin preservation?

###### Tools & Libraries
Python:
* pandas for data manipulation
* numpy for numerical operations
* plotly.express for interactive funnel visualizations
* matplotlib & seaborn for supporting visualizations

Power BI:
* KPI cards, Funnel charts, Bar charts, Matrix tables
* Slicers for interactive filtering by Category, Region, Segment, and Ship Mode

Project Steps
###### Data Preparation

* Converted numerical columns (Sales, Discount, Profit) to float
* Verified non-null values
* No major data cleaning required

###### Funnel Analysis
Stages Defined:
* Total Orders
* Discounted Orders (Discount > 0)
* High Discount Orders (Discount ≥ 20%)
* Profitable High Discount Orders (Discount ≥ 20% & Profit > 0)

###### Category-Level Funnel

* Grouped data by Category
* Calculated conversion rates for each stage:
* Discount Conversion %
* High Discount Conversion %
* Profit Conversion %

Insights:
* Furniture: High discount usage (~60%) but low profit conversion (~37%) → margin erosion
* Office Supplies: Moderate discount usage with strong profitability (~69%)
* Technology: High discount adoption with highest profit conversion (~73%) → resilient margins

Visuals:

* Interactive Plotly funnel per category
* Bar charts for profit conversion
* KPI cards for total, discounted, high-discount, and profitable orders

###### Region-Level Funnel
* Grouped data by Region
* Calculated same funnel stages and conversion metrics

###### Insights:
* West: Highest profit conversion (~78%) → sustainable discounts
* South: 100% transition from discounted → high discount orders → aggressive discounting
* Central: Lowest profit conversion (~49%) → margin risk
* East: Moderate performance

Visuals:
* Region-level funnel charts in Plotly
* Conversion rate matrix for easy comparison
* Profit conversion bar charts

###### Power BI Dashboard

Pages:

###### Category-Level Funnel Dashboard
* Funnel chart per category
* KPI cards for each stage
* Conversion matrix
* Profit leakage bar chart
* Region-Level Funnel Dashboard
* Funnel chart per region

###### KPI cards
* Conversion rate matrix
* Profit conversion bar chart
* Interactive Features:
* Slicers for Category, Region, Segment, and Ship Mode
* Drill-down for deeper insights

 ###### Key Business Insights

* Discount effectiveness varies significantly by category and region
* Blanket discounting is inefficient
* Category-specific and region-specific discount strategies maximize profitability
* Technology and Office Supplies are resilient, while Furniture is highly sensitive to discounts
* West region absorbs high discounts well; Central and East regions require careful pricing

###### Future Work / Enhancements

* Integrate time-based funnel analysis (monthly/seasonal trends)
* Predictive analytics for discount-to-profit optimization
* Incorporate customer segmentation for personalized promotions
* Extend Power BI dashboards with dynamic forecasting
