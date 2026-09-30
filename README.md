# Sales & Profitability Analysis Dashboard

An end-to-end data analytics project focused on understanding sales performance, profitability, discounting, products, countries, business segments, and yearly growth.

## Project Overview

This project follows a complete analytics workflow:

**Raw Data → Data Cleaning → Exploratory Analysis → KPI & Profitability Analysis → Power BI Dashboard → Business Recommendations**

The analysis was performed using Python and Pandas, with Excel used for data/output handling and Power BI used to build an interactive business intelligence dashboard.

## Objectives

- Clean and validate the raw sales dataset.
- Explore sales, profit, units sold, discounts, products, countries, and segments.
- Calculate key business KPIs such as profit margin and discount rate.
- Identify major sales and profitability drivers.
- Analyze performance across countries, products, business segments, years, and discount bands.
- Build an interactive Power BI dashboard.
- Translate analytical findings into actionable business recommendations.

## Dataset

The raw dataset contains **700 records and 16 original columns** covering:

- Segment
- Country
- Product
- Discount Band
- Units Sold
- Manufacturing Price
- Sale Price
- Gross Sales
- Discounts
- Sales
- COGS
- Profit
- Date
- Month Number
- Month Name
- Year

After cleaning and feature engineering, the final dataset contains **700 rows × 18 columns**.

### Engineered Features

Two additional analytical fields were created:

- **Profit Margin** = Profit / Sales
- **Discount Rate** = Discounts / Gross Sales

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Jupyter Notebook / Google Colab**
- **Microsoft Excel**
- **Microsoft Power BI**

## Data Cleaning & Preparation

The project included:

1. Inspecting dataset structure and data types.
2. Standardizing column names.
3. Checking missing values.
4. Handling missing `Discount Band` values by assigning `Unknown`.
5. Checking and removing/validating duplicate records.
6. Converting the `Date` field to datetime format.
7. Creating `Profit Margin` and `Discount Rate` metrics.
8. Validating the final cleaned dataset.

The final cleaned dataset contains **no missing values and no duplicate rows**.

## Analysis Performed

The analysis was conducted using grouped Pandas aggregations across:

### Country Analysis
Evaluated:
- Total sales
- Total profit
- Units sold
- Profit margin

### Product Analysis
Evaluated:
- Sales performance
- Profit performance
- Units sold
- Profit margin

### Segment Analysis
Evaluated:
- Sales
- Profit
- Units sold
- Loss-making segments

### Year Analysis
Evaluated:
- Yearly sales
- Yearly profit
- Units sold
- Profit margin
- Sales growth
- Profit growth

### Discount Analysis
Evaluated:
- Sales
- Discounts
- Profit
- Profit margin by discount band

## Key KPIs

| KPI | Result |
|---|---:|
| Total Sales | **$118.73M** |
| Total Profit | **$16.89M** |
| Profit Margin | **14.23%** |
| Units Sold | **1.13M** |
| Discount Rate | **7.20%** |

## Key Findings

- **United States** recorded the highest sales at approximately **$25.03M**.
- **France** recorded the highest total profit at approximately **$3.78M**.
- **Paseo** was the leading product, generating approximately **$33.01M in sales** and **$4.80M in profit**.
- The **Enterprise** segment generated approximately **$19.61M in sales but a loss of $0.61M**.
- Sales increased by approximately **249.5% from 2013 to 2014**, while profit increased by approximately **235.6%**.
- Higher discount bands were associated with lower profitability. This is an **association, not a causal conclusion**.

## Power BI Dashboard

The Power BI report contains three major sections:

### 1. Executive Overview
Provides a high-level view of:
- Total Sales
- Total Profit
- Profit Margin
- Units Sold
- Discount Rate
- Overall business performance

### 2. Performance Analysis
Provides deeper analysis of:
- Product performance
- Country performance
- Segment performance
- Yearly trends
- Sales and profitability patterns

### 3. Business Insights & Recommendations
Highlights important findings and converts them into business-focused recommendations.

## Business Recommendations

Based on the analysis:

1. Investigate **Enterprise** pricing, discounting, product mix, and cost structure.
2. Protect and expand high-performing products, particularly **Paseo**.
3. Optimize discounting while keeping profit margin as a key constraint.
4. Study the profitability drivers behind **France's** performance and identify transferable practices.
5. Investigate the products, countries, and segments contributing to the strong growth observed in **2014**.

## Project Structure

```text
Sales-and-Profitability-Analysis/
│
├── week_4_assignment.ipynb
├── sample_data_week-4.xlsx
├── Capstone_Cleaned_Data.xlsx
├── Capstone_Project_Report_Week4.pdf
├── Capstone_BI_visualization.pbix
└── README.md
