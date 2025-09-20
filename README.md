# vendor-sales-performance-python-excel-powerbi-sql

📊 Project Report: Vendor Sales & Inventory Analytics

1. Objective

The goal of this project was to analyze vendor-level sales and purchase data, identify key performance metrics, and provide insights through an interactive dashboard for better decision-making in procurement, pricing, and inventory management.


---

2. Data Sources

I worked with 6 raw CSV files (~15M+ rows, ~1GB+) containing historical records of vendor sales, purchases, inventory, and invoices:

begin_inventory.csv – Starting stock details

end_inventory.csv – Closing stock details

purchases.csv – Purchase transactions (2.3M+ rows)

purchase_prices.csv – Product price details

sales.csv – Sales transactions (12M+ rows)

vendor_invoice.csv – Vendor-wise invoice, freight, and payment details



---

3. Tools & Technologies

Python (Pandas, NumPy, Matplotlib) – Data cleaning, transformation, and EDA

SQL (SQLite) – Data integration, joins, aggregations, queries

Power BI – Dashboard creation & visualization

MS Excel – Validation and quick checks



---

4. Process & Approach

🔹 Step 1: Data Integration (ETL Pipeline)

Loaded 6 large CSV files into SQLite database for efficient querying.

Built relationships across tables using common keys (VendorNumber, InventoryId, Brand).


🔹 Step 2: Data Cleaning & Transformation

Removed duplicates, handled missing values, standardized data formats (dates, prices, sizes).

Merged purchase, sales, and inventory data to create a unified dataset.

Performed sanity checks on mismatched vendor names and prices.


🔹 Step 3: Exploratory Data Analysis (EDA)

Identified top-performing vendors based on sales & profit.

Analyzed sales trends over time and seasonality patterns.

Detected high freight cost vendors and their impact on profit margin.

Measured stock turnover and highlighted overstocked/understocked items.


🔹 Step 4: Feature Engineering (Vendor Summary Table)

Created a final vendor_sales_summary table (10K+ rows) with key KPIs:

TotalPurchaseQuantity & Dollars

TotalSalesQuantity & Dollars

Gross Profit & Profit Margin

Stock Turnover

Freight Costs

Excise Tax

Sales-to-Purchase Ratio

Vendor Performance Index


🔹 Step 5: Visualization & Reporting

Built an interactive Power BI dashboard with:

Vendor-wise profitability trends

Top 10 vendors by sales & profit

Inventory turnover & stock levels

Freight cost analysis

Year-over-year (YoY) sales comparison



---

5. Key Insights

Identified vendors with high sales but low profit margins due to high freight/excise costs.

Found underperforming vendors with low stock turnover → recommended renegotiation or discontinuation.

Highlighted vendors contributing 80% of revenue (Pareto principle).

Detected seasonal sales spikes in premium liquor brands → useful for inventory planning.



---

6. Impact & Business Value

Reduced analysis time from raw data (15M+ rows) to actionable vendor summary (~10K rows).

Provided a single source of truth for vendor performance evaluation.

Helped in data-driven decision-making for vendor contracts, pricing, and stock management.

Enhanced profitability tracking through automated KPIs & Power BI dashboards.



---

7. Tech Skills Demonstrated

Data Cleaning & Transformation (Python, Pandas, NumPy)

SQL (Joins, Group By, Aggregations, ETL)

Business Intelligence (Power BI Dashboards, DAX)

Analytical Thinking (Identifying KPIs, Business Value)



