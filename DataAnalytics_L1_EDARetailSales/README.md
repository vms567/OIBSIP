# Exploratory Data Analysis on Retail Sales Data

## Oasis Infobyte – Data Analytics Internship
**Level 1 – Task 1**

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a global bike retail sales dataset to identify sales patterns, customer behavior, product performance, and profitability trends.

The analysis focuses on transforming raw retail data into meaningful business insights that can support inventory planning, customer targeting, seasonal promotions, and product strategy.

---

## Dataset Overview

The dataset contains global bike retail sales data from 2013 to 2023.

### Initial Dataset
- Rows: 226,072
- Columns: 33
- Time Period: 2013–2023

### Important Features
- Date
- Customer Age
- Age Group
- Customer Gender
- Product Category
- Sub Category
- Product
- Order Quantity
- Unit Cost
- Unit Price
- Cost
- Revenue
- Profit
- Rating
- Insurance

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Cleaning

The following data-quality steps were performed:

- Inspected dataset shape and data types.
- Checked for missing values.
- Identified 113,011 exact duplicate rows.
- Investigated duplicate frequency before removing records.
- Removed exact duplicate records.
- Reduced the dataset from 226,072 rows to 113,061 unique records.
- Handled missing values in the `Insurance` column by assigning them to an `Unknown` category.
- Converted the `Date` column to datetime format.
- Checked important numerical fields for invalid negative values.

---

## Exploratory Data Analysis

The analysis includes:

1. Descriptive statistical analysis
2. Monthly sales revenue trend
3. Quarterly sales revenue trend
4. Customer distribution by age group
5. Customer distribution by gender
6. Top 10 best-selling products
7. Revenue by product category
8. Correlation analysis of numerical variables
9. Revenue by customer age group
10. Profit by product category

---

## Key Insights

- Adults aged 35–64 form the largest customer segment and generate the highest total revenue.
- Young Adults aged 25–34 are the second-largest customer and revenue-contributing segment.
- Water Bottle - 30 oz. is the best-selling product based on total quantity sold.
- Patch Kit/8 Patches and Mountain Tire Tube are also among the highest-selling products.
- Q2 frequently shows strong sales performance, while Q3 generally records weaker performance.
- Bikes generate substantially higher total profit than Accessories and Clothing.
- Several Accessories dominate the top-selling products by quantity, showing that high sales volume does not necessarily correspond to the highest total profitability.
- Revenue, Cost, and Profit show strong positive correlations.
- Order Quantity shows a negative relationship with Unit Price and Unit Cost, suggesting that lower-priced products tend to be purchased in larger quantities.

---

## Business Recommendations

- Maintain sufficient inventory of high-demand accessories to reduce potential stockouts.
- Prioritize profitable bike products when planning inventory, pricing, and promotional strategies.
- Prepare inventory and marketing campaigns ahead of strong Q2 demand.
- Introduce targeted promotions, bundles, or discounts to improve weaker Q3 sales.
- Prioritize Adults and Young Adults in customer-targeted campaigns while exploring opportunities to engage smaller age segments.
- Consider both sales volume and profitability when evaluating product performance.

---

## Project Structure

OIBSIP/
│
└── DataAnalytics-L1-EDARetailSales/
    │
    ├── dataset/
    │   └── bike_sales_data_world_2013_2023.csv
    │
    ├── notebook/
    │   └── Retail_Sales_EDA.ipynb
    │
    ├── outputs/
    │   └── cleaned_bike_sales_data.csv
    │
    ├── screenshots/
    │   ├── monthly_sales_trend.png
    │   ├── quarterly_sales_trend.png
    │   ├── age_group_distribution.png
    │   ├── gender_distribution.png
    │   ├── top_10_products.png
    │   ├── revenue_by_category.png
    │   ├── correlation_heatmap.png
    │   ├── revenue_by_age_group.png
    │   └── profit_by_category.png
    │
    └── README.md

---

## Conclusion

The EDA revealed meaningful patterns in sales performance, customer demographics, product demand, and profitability.

The results highlight strong seasonal variations, the importance of adult customer segments, high demand for cycling accessories, and the strong profitability of the Bikes category.

These findings can support data-driven decisions related to inventory management, marketing campaigns, customer segmentation, seasonal planning, and product strategy.

---

## Author

**Vikas Gaikwad**

Data Analytics Intern – Oasis Infobyte