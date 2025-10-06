# Walmart Data Analysis SQL+Python Project

 Project Overview:
![image alt](https://github.com/siddheshdesai/Walmart_SQL_Python/blob/6fa1f79307b8e7b9057f166287ddfc6e493d91a4/walmart_project-pipelines.png)


This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. We utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve key business questions. The project is ideal for data analysts looking to develop skills in data manipulation, SQL querying, and data pipeline creation.



# Project Steps
## 1. Set Up the Environment
* Tools Used: Visual Studio Code (VS Code), Python, SQL (MySQL and PostgreSQL)
* Goal: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.

## 2. Set Up Kaggle API
* API Setup: Obtain your Kaggle API token from Kaggle by navigating to your profile settings and downloading the JSON file.
* Configure Kaggle:
   - Place the downloaded kaggle.json file in your local .kaggle folder.
   - Use the command kaggle datasets download -d <dataset-path> to pull datasets directly into your project.
## 3.Download Walmart sales data
* Data Source: Use the Kaggle API to download the Walmart sales datasets from Kaggle.
* Dataset Link: https://www.kaggle.com/datasets/najir0123/walmart-10k-sales-datasets
* Storage: Save the data in the data/ folder for easy reference and access.

## 4.Install Required Libraries and Load Data
* Libraries: Install necessary Python libraries using:
<pre lang="markdown"> bash pip install pandas numpy sqlalchemy mysql-connector-python psycopg2 </pre>

## 5. Explore the Data
* Goal: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
* Analysis: Use functions like .info(), .describe(), and .head() to get a quick overview of the data structure and statistics.

## 6. Data Cleaning
* Remove Duplicates: Identify and remove duplicate entries to avoid skewed results.
* Handle Missing Values: Drop rows or columns with missing values if they are insignificant; fill values where essential.
* Fix Data Types: Ensure all columns have consistent data types (e.g., dates as datetime, prices as float).
* Currency Formatting: Use .replace() to handle and format currency values for analysis.
* Validation: Check for any remaining inconsistencies and verify the cleaned data.

## 7. Feature Engineering
- **Create New Columns:** Calculate the **Total Amount** for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.  
- **Enhance Dataset:** Adding this calculated field streamlines further SQL analysis and aggregation tasks.

---

## 8. Load Data into MySQL and PostgreSQL
- **Set Up Connections:** Connect to **MySQL** and **PostgreSQL** using `sqlalchemy` and load the cleaned data into each database.  
- **Table Creation:** Set up tables in both databases using Python **SQLAlchemy** to automate table creation and data insertion.  
- **Verification:** Run initial SQL queries to confirm accurate data loading.

---

## 9. SQL Analysis: Complex Queries and Business Problem Solving
**Business Problem-Solving:** Execute complex SQL queries to address key business questions, such as:
- Revenue trends across branches and categories  
- Identifying best-selling product categories  
- Sales performance by time, city, and payment method  
- Analyzing peak sales periods and customer buying patterns  
- Profit margin analysis by branch and category  

**Documentation:** Keep clear notes for each query's objective, approach, and results.

---

## 10. Project Publishing and Documentation
- **Documentation:** Maintain detailed documentation in Markdown or Jupyter Notebook.  
- **Project Publishing:** Publish the project on GitHub including:
  - `README.md` (this document)
  - Jupyter Notebooks (if applicable)
  - SQL Query Scripts
  - Data files or download instructions
  - `requirements.txt` (library dependencies)

---

## ⚙️ Requirements

**Python Version:** 3.8+  
**Databases:** MySQL, PostgreSQL  
**Python Libraries:**
- pandas
- numpy
- sqlalchemy
- mysql-connector-python
- psycopg2
  
**Kaggle API Key (for dataset downloading)**







##  Getting Started

1️⃣ Clone the repository
<pre lang="markdown">
 git clone repo-url
</pre>


2️⃣ Install Python libraries
<pre lang="markdown">
pip install -r requirements.txt
</pre>

3️⃣ Setup your Kaggle API, download the data, and follow the steps to load and analyze.


## Project Structure
<pre lang="markdown">

|-- data/                     # Raw data and transformed data
|-- sql_queries/              # SQL scripts for analysis and queries
|-- notebooks/                # Jupyter notebooks for Python analysis
|-- README.md                 # Project documentation
|-- requirements.txt          # List of required Python libraries
|-- main.py                   # Main script for loading, cleaning, and processing data
</pre>

📊 Results and Insights

This section summarizes your analysis findings:

- Sales Insights: Key categories, top-performing branches, and preferred payment methods.
- Profitability: Most profitable product categories and locations.
- Customer Behavior: Patterns in ratings, payment preferences, and peak shopping hours.

## Future Enhancements
Possible extensions to this project:

- Integration with a dashboard tool (e.g., Power BI or Tableau) for interactive visualization.
- Additional data sources to enhance analysis depth.
- Automation of the data pipeline for real-time data ingestion and analysis.

## Acknowledgments
- Data Source: Kaggle’s Walmart Sales Dataset
- Inspiration: Walmart’s business case studies on sales and supply chain optimization.
