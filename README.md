# Superstore Sales & Profitability Analysis

## 1. Project Overview

This project focuses on analysing retail sales and profitability using the Sample Superstore dataset. The objective is to understand business performance across product categories, sub-categories, customers, discounts, and shipping operations.

The project follows an end-to-end data analysis workflow involving Python for data preparation, PostgreSQL for database management, and Power BI for interactive dashboard development.

The analysis identifies sales trends, profitability patterns, loss-making products, and the impact of discount strategies on business performance.

## 2. Problem Statement

Retail businesses need to understand which products and categories generate profits and which contribute to financial losses.

Excessive discounting, differences in product performance, and shipping operations can influence overall profitability.

This project investigates sales performance, identifies loss-making sub-categories, examines the relationship between discounts and profit, and analyses shipping duration to uncover opportunities for better business decisions.

## 3. Tools & Technologies

- **Python (Pandas):** Data loading, inspection, and preprocessing.
- **PostgreSQL:** Database storage and SQL-based data analysis.
- **Power BI:** Interactive dashboard development and data visualization.
- **CSV:** Dataset storage and data exchange.
- **GitHub:** Project documentation and version control.

## 4. Dataset Information

- **Dataset Name:** Sample Superstore
- **Dataset Source:** Kaggle – Sample Superstore
- **File Name:** Sample - Superstore.csv
- **Total Records:** 9,994
- **Total Columns:** 21

### Dataset Attributes

The dataset contains retail transaction information, including:

- Order ID and Order Date
- Ship Date and Ship Mode
- Customer ID and Customer Name
- Segment
- Country, City, State, Postal Code, and Region
- Product ID, Category, Sub-Category, and Product Name
- Sales, Quantity, Discount, and Profit

**Dataset Source:** [Kaggle – Sample Superstore](https://www.kaggle.com/datasets/vivek468/superstore-dataset-fi)

## 5. Data Preprocessing

Python and Pandas were used to inspect and prepare the dataset.

The following preprocessing activities were performed:

1. Loaded the dataset and examined its structure.
2. Checked dataset dimensions, column names, and data types.
3. Checked for missing values.
4. Examined the dataset for duplicate records.
5. Verified Order Date and Ship Date formats.
6. Created a calculated column named `shipping_days`.
7. Calculated shipping duration by subtracting Order Date from Ship Date.
8. Examined shipping duration statistics.
9. Prepared the dataset for PostgreSQL storage and Power BI analysis.

### Shipping Duration Statistics

- Total Records: 9,994
- Average Shipping Duration: 3.96 days
- Minimum Shipping Duration: 0 days
- Maximum Shipping Duration: 7 days

## 6. Database Management

PostgreSQL was used to store the prepared dataset in a table named `superstore`.

The dataset was imported into PostgreSQL and used for structured data analysis.

The database provided a foundation for querying and examining sales, profit, discounts, product categories, and shipping information.

## 7. Analysis Performed

### A. Overall Business Performance
- Analysed total sales and total profit.
- Evaluated total orders and customer count.
- Calculated overall profit margin.
- Examined total quantity sold.

### B. Category & Sub-Category Analysis
- Compared sales and profit across Furniture, Technology, and Office Supplies.
- Identified high-performing and low-performing categories.
- Examined sub-categories contributing to business losses.

### C. Discount & Profitability Analysis
- Examined the relationship between discount percentages and profit.
- Identified discount levels associated with negative profitability.
- Evaluated the impact of higher discounts on profit margins.

### D. Product Loss Analysis
- Identified products and sub-categories generating negative profits.
- Examined major contributors to product-level losses.
- Investigated opportunities to improve profitability.

### E. Shipping Analysis
- Examined shipping duration across orders.
- Analysed shipping days to understand delivery patterns.

## 8. Key Findings & Business Insights

### Overall Business Performance

| KPI | Result |
|---|---:|
| Total Sales | $2,297,200.86 |
| Total Profit | $286,397.02 |
| Total Orders | 5,009 |
| Total Customers | 793 |
| Total Quantity | 37,873 |
| Profit Margin | 12.47% |

### Category Performance

- **Technology:** Generated the highest category profit of $145,454.95, with a 17.40% profit margin.
- **Office Supplies:** Generated $122,490.80 in profit, with a 17.04% profit margin.
- **Furniture:** Recorded a comparatively low profit margin of 2.49%.

### Loss-Making Sub-Categories

- Tables recorded a loss of $17,725.48.
- Bookcases recorded a loss of $3,472.56.
- Supplies recorded a loss of $1,189.10.

### Discount Impact on Profitability

The analysis revealed a declining profit margin at higher discount levels.

| Discount | Profit Margin |
|---|---:|
| 0% | 18.55% |
| 20% | -0.67% |
| 30% | -13.51% |
| 40% | -35.49% |
| 45% | -45.45% |
| 50% | -63.00% |

These findings highlight the importance of reviewing discount strategies and monitoring loss-making products to improve retail profitability.

## 9. Power BI Dashboard Screenshots

### Overall Business Performance

![Dashboard Overview](screenshots/dashboard-overview.png)

### Category & Sub-Category Profitability

![Category Profitability](screenshots/category-profitability.png)

### Discount & Profit Analysis

![Discount Profit Analysis](screenshots/discount-profit-analysis.png)

### Additional Dashboard Analysis

![Additional Analysis](screenshots/additional-analysis.png)

## 10. Project Workflow

1. Dataset collection and loading.
2. Data inspection and preprocessing using Python.
3. Database creation and data storage using PostgreSQL.
4. Data analysis and exploration.
5. Interactive dashboard development using Power BI.
6. Business insights and findings.

## 11. Conclusion

This project demonstrates an end-to-end retail data analysis workflow involving Python, PostgreSQL, and Power BI.

The analysis provides insights into sales performance, category profitability, discount strategies, shipping duration, and loss-making products.

The findings help identify areas where businesses can review pricing and discount decisions, monitor product performance, and improve overall profitability.
