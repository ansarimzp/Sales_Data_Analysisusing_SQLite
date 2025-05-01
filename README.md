# 📊 Sales Data Analysis with SQLite & Python
This project demonstrates an end-to-end analysis of sales data using SQLite for database management and Python for data manipulation & visualization. The Jupyter notebook provides a clear workflow from data ingestion to actionable insights, leveraging SQL queries within Python for seamless analysis.

# 🚀 Key Features
## 1. Data Integration & SQLite Database
Import & Preview Data: Load a cleaned sales dataset (cleaned_train.csv) into a Pandas DataFrame.

### SQLite Database Setup: Convert the DataFrame into an SQLite database (sales_data.db) with a sales table for efficient querying.

## 2. Advanced SQL Analytics
### Revenue Rankings: Identify top-selling products by revenue (e.g., Canon copiers, Fellowes punch binders).

### Sales Trends: Analyze sales performance by product, region, or customer segment using SQL aggregations.

### Query Examples:
-- Top 10 products by revenue
SELECT "Product Name" AS product, SUM(Sales) AS revenue 
FROM sales 
GROUP BY product 
ORDER BY revenue DESC 
LIMIT 10;
## 3. Interactive Visualizations
Horizontal Bar Plots: Visualize top products by revenue using matplotlib.

Customizable Metrics: Easily modify the code to compare sales by category, region, or time period.

## 4. Exploratory Data Analysis (EDA)
Explore raw data structure, including columns like Order ID, Customer Segment, Product Category, and Sales.

Clean and preprocess data for analysis-ready formatting.

## ⚙️ Setup & Usage
Dependencies
pip install sqlite3 pandas matplotlib itertools collections
Steps
Update CSV Path:
Replace the CSV file path in the notebook with your dataset location:


df = pd.read_csv(r"C:\Users\altam\Documents\cleaned_train.csv")  # Modify this path
Run the Notebook:
Execute cells sequentially to:

Create the SQLite database

Perform SQL queries

Generate visualizations

## 📂 Database Schema
Table Name: sales
Columns:

Row ID, Order ID, Order Date, Ship Date, Ship Mode, Customer ID, Customer Name, Segment, Country, City, State, Postal Code, Region, Product ID, Category, Sub-Category, Product Name, Sales

## 🔍 Key Insights (Example)
Top Product: "Canon imageCLASS 2200 Advanced Copier" generated $61,599.82 in revenue.

Regional Trends: Deep-dive into geographic performance (e.g., Southern U.S. vs. Western U.S.).

Customer Segmentation: Compare sales across consumer, corporate, and home office segments.




## 💡 Future Enhancements
Add time-series analysis (monthly/yearly sales trends).

Integrate customer lifetime value (CLV) calculations.

Build a dashboard with Plotly or Tableau for interactive reporting.

## 🛠️ Tools Used
Python Libraries: Pandas, SQLite3, Matplotlib

Database: SQLite

Data Source: Custom sales dataset (cleaned_train.csv)

👨💻 Author: Altamash Ali Ansari 
📧 Contact: ansarimzp63@gmail.com
