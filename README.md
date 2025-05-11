# E-commerce Data Analysis with Python and SQL

## Project Description

This project focuses on analyzing e-commerce data using Python for data manipulation, visualization, and interacting with a SQL database. The goal is to extract insights from e-commerce transactions, customers, products, and sales data through SQL queries and Python scripting.

## Files Included

* `csv_to_sql.py`: A Python script designed to read CSV files (assumed to be the raw data) and load them into appropriate tables in a MySQL database.
* `Python + SQL E-commerce.ipynb`: A Jupyter Notebook containing the core analysis. It includes Python code for connecting to the database, executing SQL queries, performing data processing with pandas, and creating visualizations with matplotlib/seaborn.
* `Python + SQL E-commerce.pdf`: A static PDF export of the Jupyter Notebook, providing a view of the analysis and its output without needing to run the notebook.
* `Questions.txt`: A text file listing various SQL queries of varying complexity (Basic, Intermediate, Advanced) related to e-commerce data, which served as prompts for the analysis.

## Prerequisites

To run this project locally, you will need:

* Python 3.x
* `pip` package installer
* MySQL Database server running
* E-commerce dataset in CSV format (specifically: `customers.csv`, `orders.csv`, `sales.csv`, `products.csv`, `delivery.csv`, `payments.csv` as indicated in `csv_to_sql.py`). **Note:** The CSV files themselves are not included in this repository and must be obtained separately.
* Jupyter Notebook or JupyterLab (for running the `.ipynb` file)

## Setup and Installation
1.  **Install Python Libraries:**
    ```bash
    pip install pandas mysql-connector-python matplotlib seaborn jupyter
    ```

2.  **Database Setup:**
    * Ensure your MySQL server is running.
    * Create a database (e.g., named `ecommerce`).
    * Update the database connection details (`host`, `user`, `password`, `database`) in both `csv_to_sql.py` and `Python + SQL E-commerce.ipynb` to match your MySQL setup. **Caution:** Do not hardcode sensitive passwords if sharing publicly; consider using environment variables or a separate config file ignored by Git for real projects. For this example, placeholder text is used.

3.  **Data Loading:**
    * Place your e-commerce CSV files (`customers.csv`, `orders.csv`, etc.) into a folder.
    * Update the `folder_path` variable in `csv_to_sql.py` to the path of this folder.
    * Run the script to load data into the database:
        ```bash
        python csv_to_sql.py
        ```

## Usage

1.  **Run the Data Loading Script:** Execute `python csv_to_sql.py` first to populate your database with the data from the CSV files.
2.  **Explore the Analysis:** Open the Jupyter Notebook:
    ```bash
    jupyter notebook "Python + SQL E-commerce.ipynb"
    ```
    Run the cells sequentially to see the SQL queries executed, data processed with pandas, and the resulting visualizations.
3.  **Review the Queries:** Consult `Questions.txt` for a list of the specific analysis questions addressed in the project.
4.  **View the Static Report:** Open `Python + SQL E-commerce.pdf` to see a static version of the notebook's output.

## Analysis Highlights

The project performs various analyses, including:

* Listing unique customer cities.
* Counting orders in specific years.
* Calculating total sales per product category.
* Analyzing payment methods (installments).
* Counting customers per state.
* Analyzing monthly order trends.
* Calculating average products per order by city.
* Identifying top customers by spending.
* Calculating customer retention rate.
* *...and more, as detailed in the Jupyter Notebook.*

## Technologies Used

* Python
* SQL (MySQL)
* pandas
* matplotlib
* seaborn
* Jupyter Notebook

