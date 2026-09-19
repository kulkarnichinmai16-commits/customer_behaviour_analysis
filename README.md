This project demonstrates an end-to-end Data Analytics workflow, starting from loading and understanding the dataset to data cleaning, exploratory data analysis (EDA), SQL analysis, dashboard creation, and presenting the final insights.

The project uses Python, SQL, PostgreSQL/MySQL/SQL Server, and Power BI to transform raw data into meaningful business insights.

A final analytical report and PowerPoint presentation created using Gamma are also included to communicate the findings clearly.

🎯 Project Objectives
Load and understand the dataset using Python
Clean and prepare raw data for analysis
Perform Exploratory Data Analysis (EDA)
Identify important patterns and trends
Perform business analysis using SQL
Store and query data using PostgreSQL/MySQL/SQL Server
Create an interactive Power BI dashboard
Generate a detailed analytical report
Present key findings using a professional PPT


📂 Dataset

The project uses a structured dataset containing relevant business/customer/sales information.

The dataset was initially loaded into Python for:

Understanding data structure
Checking missing values
Identifying duplicate records
Checking incorrect data types
Detecting inconsistent values
Understanding numerical and categorical columns

Dataset: customer_shopping_behaviour.csv

🛠️ Tools & Technologies
Tool	Purpose
Python	Data loading, cleaning and EDA
Pandas	Data manipulation and analysis
NumPy	Numerical operations
Matplotlib / Seaborn	Data visualization
PostgreSQL / MySQL / SQL Server	SQL analysis and database management
SQL	Data querying and business analysis
Power BI	Interactive dashboard creation

Excel / CSV	Dataset handling
🔄 Project Workflow
Raw Dataset
     ↓
Load Dataset in Python
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis (EDA)
     ↓
Load Data into SQL Database
     ↓
SQL Queries & Analysis
     ↓
Power BI Dashboard
     ↓
Analytical Report
     ↓
Gamma PPT Presentation
     ↓
Business Insights
🐍 1. Data Loading Using Python

The dataset is loaded into Python using Pandas.

Example:

import pandas as pd

df = pd.read_csv("dataset.csv")

print(df.head())
print(df.shape)
print(df.info())

The initial analysis helps understand:

Number of rows and columns
Column names
Data types
Missing values
Duplicate records
Basic statistics
🧹 2. Data Cleaning

The raw dataset is cleaned before performing further analysis.

Major cleaning activities include:

Handling missing values
Removing duplicate records
Correcting data types
Handling inconsistent values
Renaming columns where required
Removing unnecessary columns
Formatting date and numerical fields
Checking for invalid or unusual values

Example:

df.isnull().sum()
df.duplicated().sum()

After cleaning, the dataset is prepared for analysis and SQL processing.

📊 3. Exploratory Data Analysis (EDA)

EDA is performed using Python to understand the data and identify important patterns.

The analysis includes:

Descriptive statistics
Distribution analysis
Category-wise analysis
Trend analysis
Correlation analysis
Outlier identification
Business-related KPIs

Visualization libraries such as Matplotlib and Seaborn are used to create charts and graphs.

🗄️ 4. SQL Analysis

The cleaned dataset is imported into a relational database such as:

PostgreSQL
MySQL
SQL Server

SQL queries are then used to perform business analysis.

Examples of analysis include:

-- Total records
SELECT COUNT(*) 
FROM customers;

-- Total sales
SELECT SUM(sales) AS total_sales
FROM sales;

-- Average sales
SELECT AVG(sales) AS average_sales
FROM sales;

-- Top products
SELECT product_name, SUM(sales) AS total_sales
FROM sales
GROUP BY product_name
ORDER BY total_sales DESC;

Other SQL concepts used include:

SELECT
WHERE
GROUP BY
HAVING
ORDER BY
DISTINCT
Aggregate functions
CASE statements
JOINs
Subqueries
CTEs
Window functions
📈 5. Power BI Dashboard

An interactive Power BI dashboard is created to present the important findings visually.

Dashboard Includes
Total Sales
Total Customers
Total Orders
Average Sales
Sales Trends
Top Products
Category-wise Performance
Customer Analysis
Regional/Location Analysis
Interactive filters and slicers

The dashboard allows users to explore the data and understand important business trends quickly.
<img width="1151" height="627" alt="image" src="https://github.com/user-attachments/assets/74e8a5e8-0c8e-4724-b6be-5d569881a378" />


