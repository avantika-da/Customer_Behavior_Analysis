Data Analytics Portfolio Project: Customer_Behavior_Analysis

Overview

This project focuses on a complete end-to-end data analytics pipeline, from data ingestion and cleaning in Python to advanced data storage, query execution in PostgreSQL, and final visualization in a dynamic Power BI Dashboard. The primary objective was to analyze historical sales data to uncover key performance indicators (KPIs), identify potential areas for optimization, and present actionable insights.

This project demonstrates proficiency in data manipulation, database management, business intelligence visualization, and executive reporting.

Dataset

Source: Mock company sales data (e.g., Global Superstore Dataset).

Content: Contains over 3,900 records of individual transactions, including product details, customer demographics, regional sales performance, shipping logistics, and profit margins.

Key Metrics Analyzed: Total Revenue, Profit Margin by Region/Category, Customer Segmentation, and Order Fulfillment Efficiency.

Tools and Technologies

Category

Tool / Library

Purpose

Data Processing & Analysis

Python 3.x

Core scripting language



Pandas, NumPy

Data ingestion, cleaning, manipulation, and Exploratory Data Analysis (EDA)

Database Management

PostgreSQL

Relational database for scalable storage and complex querying



Psycopg2 / SQLAlchemy

Python library for database connectivity and loading

Business Intelligence

Power BI

Creating interactive and professional data visualizations and dashboards

Reporting & Presentation

Gamma / Microsoft PowerPoint

Producing the final analytical report and executive summary presentation

Querying

SQL (PostgreSQL dialect)

Executing complex joins, aggregations, and data retrieval

Project Steps and Methodology

The project followed a standard, robust data analysis lifecycle:

Data Ingestion & Cleaning (Python):

Loaded the raw CSV data into a Pandas DataFrame.

Handled missing values (imputation/removal) and removed duplicate records.

Standardized text fields and corrected data types (e.g., converting 'Sales' column to numeric float).

Engineered new features (e.g., Profit_Ratio, Order_to_Ship_Days).

Exploratory Data Analysis (EDA) (Python):

Calculated descriptive statistics to understand data distribution.

Identified outliers and anomalies (e.g., negative profit).

Visualized key relationships using Matplotlib/Seaborn (e.g., sales vs. region, correlation heatmaps).

Database Loading & Querying (PostgreSQL & SQL):

The cleaned DataFrame was uploaded to a local PostgreSQL server instance.

Designed and executed complex SQL queries to pre-aggregate data for the dashboard. Queries included JOIN operations, WINDOW FUNCTIONS, and GROUP BY aggregations (e.g., calculating running profit totals per quarter).

Data Visualization (Power BI):

Connected Power BI directly to the PostgreSQL database.

Designed a multi-page interactive dashboard focusing on key business questions.

Applied DAX calculations to create advanced time intelligence and rank measures.

Final Reporting (Report & Gamma PPT):

Summarized the entire project, methodology, and key findings in a formal Analytical Report.

Created a high-impact, visual Executive Summary Presentation (Gamma) for key stakeholders, translating complex data insights into clear business recommendations.

Power BI Dashboard Highlights

The final dashboard provides a comprehensive view of business performance, enabling stakeholders to filter and drill down into specific areas:

Geographic Performance: Interactive map showing sales and profit by state and city.

Category Deep Dive: Treemap visualization detailing product-level profit and loss.

Time Series Analysis: Dual-axis charts tracking quarterly sales growth and profit margin trends.

Efficiency Metrics: Card visuals displaying average shipping time and return rate.

Key Results and Business Insights

Regional Focus: Identified that the Central region, while having high sales volume, consistently maintained a 15% lower profit margin due to inefficient logistics. Recommendation: Review shipping carrier contracts in the Central region.

Product Opportunity: The 'Office Supplies' category drives 45% of total transactions but contributes only 20% to the total profit. Recommendation: Implement targeted pricing adjustments for low-margin office supply subcategories.

Customer Loyalty: Analysis of repeat purchases revealed that the top 5% of customers contribute 35% of overall profit.

How to Run This Project

To replicate the project's data preparation and database loading locally:

Prerequisites: Ensure you have Python 3.x, PostgreSQL, and Power BI installed.

Setup Environment: Clone the repository and install necessary Python libraries:

pip install pandas numpy psycopg2-binary


Database Configuration:

Ensure your PostgreSQL server is running.

Update the connection string details (host, database name, user, password) in the data_cleaning.py script.

Execute Python Script: Run the main data preparation script to clean the data and load it into PostgreSQL:

python data_cleaning.py


View Dashboard: Open the customer_shopping_behavior.pbix file in Power BI and refresh the data connection, pointing it to your local PostgreSQL instance.
