**📌 Project Overview**
This project demonstrates an end-to-end data engineering and analytics workflow using a multi-table E-commerce dataset. It focuses on automating the data migration process from raw CSV files to a structured MySQL database using Python and subsequently performing deep-dive SQL analysis to extract actionable business insights.

**🛠️ Technical Stack**
**Language:** Python

**Database:** MySQL

**Libraries:** Pandas (Data Manipulation), mysql-connector-python (Database Connectivity), Matplotlib & Seaborn (Visualization)

**Tools:** MySQL Workbench, Jupyter Notebook

**📂 Dataset Architecture**
The project utilizes seven interconnected datasets representing a comprehensive e-commerce ecosystem:

**customers.csv:** Unique identifiers and geographic distribution of customers.

**orders.csv:** Transactional data including timestamps and delivery status.

**order_items.csv:** Detailed product-level information for each order.

**products.csv:** Product categories and physical dimensions.

**payments.csv:** Payment methods, installments, and transaction values.

**sellers.csv:** Seller locations and identifiers.

**geolocation.csv:** Precise mapping data for logistics analysis.

**🚀 Key Features & Workflow**
**1. Automated Data Pipeline (Python)**
Dynamic Table Creation: A custom Python script that iterates through the CSV files, cleans column names, and automatically generates SQL CREATE TABLE statements with appropriate data types.

Efficient Data Loading: Handles NaN values and inserts thousands of records into the MySQL database using the mysql-connector interface.

**2. Advanced SQL Analytics**
The core analysis focuses on 15+ complex business queries, including:

**Customer Geography:** Identifying the top 10 cities by customer volume.

**Sales Performance:** Analyzing total revenue trends across product categories.

**Financial Insights:** Calculating the percentage of orders paid via installments.

**Retention Analysis:** Measuring customer retention by identifying repeat purchases within 6-month intervals.

**High-Value Ranking:** Using Window Functions (DENSE_RANK()) to identify the top 3 spending customers per year.

**3. Data Visualization**
Integrated Python visualizations (Bar plots) to represent complex SQL query results, such as yearly spending leaders, making the data accessible for stakeholders.

**📈 Key Insights Generated**
**Urban Concentration:** Identification of high-volume hubs like São Paulo and Rio de Janeiro for targeted marketing.

**Payment Trends:** Understanding consumer reliance on installment plans to optimize financial offerings.

**Category Leadership:** Data-driven ranking of top-performing product categories to inform inventory management.

**How to Run**
Ensure you have a local MySQL instance running.

Update the database credentials in the Python+MySQL_Ecommerce.ipynb notebook.

Run the notebook to initialize the database and load the datasets.

Execute the queries in MySQL Queries Required.sql via MySQL Workbench for manual analysis.
