# orders-data-sql-pipeline
# Data Analysis Pipeline: From Kaggle to SQL Server

This project demonstrates a complete data pipeline starting from downloading a dataset using the **Kaggle API**, followed by **data cleaning and processing using Python (Pandas)**, loading the cleaned data into **SQL Server**, and performing **data analysis using SQL**.

---

## 📊 Workflow Overview

![workflow diagram](https://github.com/user-attachments/assets/09f465b3-ce5d-4245-9e06-e24649f35efe)


### 1. 📥 Download Dataset (Kaggle API)
- The dataset is downloaded programmatically using the Kaggle API.
- You must have your Kaggle API token configured in your environment.

### 2. 🧹 Data Cleaning & Processing (Python - Pandas)
- The raw data is cleaned and transformed using **Pandas**.
- Steps include:
  - Handling missing values
  - Renaming columns
  - Calculating new columns (e.g., `discount`, `sale_price`, `profit`)
  - Formatting dates

### 3. 🗃 Load Data to SQL Server
- The cleaned DataFrame is loaded into **Microsoft SQL Server** using SQLAlchemy or pyodbc.
- Ensure SQL Server is running and accessible with the correct driver.

### 4. 📈 Data Analysis using SQL
- Various SQL queries are used to:
  - Identify top-selling products by region
  - Analyze monthly trends
  - Compare year-over-year sales

---

## 🔧 Tech Stack

| Tool        | Purpose                          |
|-------------|----------------------------------|
| Python      | Scripting and data manipulation  |
| Pandas      | Data cleaning and transformation |
| SQLAlchemy  | Connecting to SQL Server         |
| SQL Server  | Data storage and analysis        |
| Kaggle API  | Dataset download                 |

---

## ▶️ How to Run

1. Clone the repository  
2. Set up your Kaggle API key  
3. Install dependencies:  
   ```bash
   pip install pandas sqlalchemy kaggle pyodbc
