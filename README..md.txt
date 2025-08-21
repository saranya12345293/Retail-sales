Retail Sales Data Analysis
1. Project Overview

This project analyzes retail sales data to identify key performance indicators (KPIs), trends, and patterns.
The process includes:

Data Cleaning (removing errors, fixing missing values)

Exploratory Data Analysis (EDA) (basic sales trends & summaries)

Advanced Analysis (profitability, rankings, growth trends)

The goal is to demonstrate SQL skills for real-world business analytics.

2. Dataset Description

The dataset contains sales transactions from a retail store.
Key columns:

transactions_id – Unique transaction reference

customer_id – Customer identifier

category – Product category (e.g., clothing, electronics)

gender – Customer gender

age – Customer age

quantity – Number of items sold

price_per_unit – Price per item

cogs – Cost of goods sold

total_sale – Total revenue from transaction

sale_date – Date of sale

sale_time – Time of sale

3. Data Cleaning Steps

Remove invalid data – Deleted rows where quantity or price were zero/negative.

Fill missing values – Estimated missing cogs using (price * quantity * 0.7).

Standardize text fields – Converted category to lowercase & trimmed spaces.

Remove duplicates – Ensured each transactions_id is unique.

Ensure date format – Standardized sale_date to YYYY-MM-DD.

4. Exploratory Data Analysis (EDA)

Total sales by category – Found top-performing product categories.

Sales by gender – Compared revenue between male and female customers.

Age group sales – Grouped customers into age ranges and analyzed spending.

Monthly sales trend – Summarized sales per month to identify seasonality.

Top customers – Ranked customers by total spending.

Peak sales hours – Found the busiest sales hours.

Average quantity per category – Checked purchasing patterns per category.

5. Advanced Analysis

Profit by category – Calculated profit using (total_sale - cogs).

Rank categories – Used SQL RANK() to rank by sales volume.

Year-over-Year growth – Compared yearly revenue growth in percentage.

Top 10 customers – Listed highest-spending customers.

Profit margin per category – Calculated average percentage profit margin.

6. Key Insights

Top categories drive over 60% of total revenue.

Female customers tend to spend slightly more than male customers in certain categories.

Ages 30–39 are the highest-spending group.

Monthly trend shows peak sales in holiday months (Nov–Dec).

Year-over-year growth is positive, indicating business expansion.

7. How to Run in DB Browser

Open DB Browser for SQLite.

Go to File → New Database → Save it.

Go to File → Import → Table from CSV/Excel → Select your Excel data.

Name the table sales.

Open Execute SQL tab.

Paste queries from queries.sql in order:

Data Cleaning → Run

EDA Queries → Run each separately to see results

Advanced Analysis → Run for deeper insights

Export results if needed to CSV for visualization.