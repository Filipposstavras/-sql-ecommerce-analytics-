# E-Commerce Sales & Customer Analytics
_SQL • Python • Power BI_

This project showcases end-to-end analytics on a small e-commerce dataset using SQL, Python, and Power BI.  
It demonstrates both basic and advanced SQL queries, automated data loading with Python, and visualization readiness for BI tools.  

------------------------------------------------------------
Key Skills Demonstrated
- Database design & querying
  - Normalized schema with customers, products, orders, order_items, payments
  - Joins, GROUP BY, window functions, CTEs, and aggregates
- Analytical SQL
  - Revenue trends
  - Customer lifetime value (LTV)
  - Average order value (AOV)
  - Refund rates
  - Repeat purchase rate
  - Cohort analysis
  - Market-basket analysis (product pairs)
  - Retention metrics
- Python integration
  - Data loading with pandas + SQLAlchemy
  - Scripted schema creation and seed data insertion
  - Export of query results as CSV for BI tools
- Power BI dashboarding
  - Revenue, category share, AOV by country
  - Top customers and product pairs
  - Direct import of exported CSVs into interactive dashboards

------------------------------------------------------------
Business Questions Answered
- Monthly revenue & orders
- Revenue by category + share of total
- Top 10 customers by LTV
- AOV by country
- Refund rate (%) by month
- Repeat purchase rate
- First product purchased by new customers (signup cohorts)
- Product pairs frequently bought together
- Median time to second order
- 7-day moving average of revenue

------------------------------------------------------------
Tech Stack
- SQL: PostgreSQL (schema + queries), SQLite (demo)
- Python: pandas, SQLAlchemy
- BI: Power BI (CSV import + visuals)

------------------------------------------------------------
How to Run
- Clone the repository
  - git clone https://github.com/Filipposstavras/sql-ecommerce-analytics.git
  - cd sql-ecommerce-analytics

- (Optional) Create a virtual environment
  - python -m venv .venv
  - source .venv/bin/activate   (Windows: .venv\Scripts\activate)

- Install dependencies
  - pip install -r requirements.txt

- Load schema and seed data
  - python load_and_run.py
  - This will create the database (SQLite by default) and insert the CSV seed data

- Run SQL queries
  - Open queries.sql in your SQL client (PostgreSQL or SQLite)
  - Execute the queries to generate insights

- Review exports
  - Query results are also available in the /exports folder as CSV files
  - These files can be directly imported into Power BI

- Build Power BI dashboards
  - Import CSVs from /exports
  - Suggested visuals:
    - Line chart: monthly revenue (with 7-day MA)
    - Bar chart: revenue by category + % share
    - Bar chart: AOV by country
    - Table: Top 10 customers by LTV
    - Matrix: product pairs frequently bought together
