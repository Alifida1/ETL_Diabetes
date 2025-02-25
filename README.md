**ETL Pipeline: MongoDB to PostgreSQL for Diabetes Data**
**Project Overview**

This project implements an ETL (Extract, Transform, Load) pipeline that extracts diabetes patient data from MongoDB, processes and transforms it in Jupyter Notebook, and finally loads the cleaned dataset into a PostgreSQL database. The goal was to explore and enhance data usability by applying transformations that improve interpretability and analytical insights.

**Objectives**

> Extract data from MongoDB.

> Perform exploratory data analysis (EDA) to understand the dataset.

> Transform key variables for better interpretability.

> Load the processed data into PostgreSQL for structured storage and querying.

**Data Extraction**

The diabetes dataset was stored in MongoDB. Using Python’s pymongo library, the data was extracted and loaded into a Pandas DataFrame for further processing.

**Data Transformation**

Key transformations included:

**Age Categorization:** Numeric values were mapped to human-readable age groups.

**Education Level Mapping:** Education levels were replaced with more intuitive labels.

**Income Classification:** Income was categorized into Low, Medium, and High groups.

**Exploratory Data Analysis (EDA):** Distribution plots, correlation matrices, and category counts were used to gain insights.

**Data Loading**

The transformed dataset was loaded into PostgreSQL using SQLAlchemy. The _id column (from MongoDB) was removed to ensure compatibility with PostgreSQL.

**Tools & Technologies Used**

**Database Systems:** MongoDB, PostgreSQL

**Programming Language:** Python

**Libraries:** Pandas, PyMongo, SQLAlchemy, Matplotlib, Seaborn

**Conclusion**
This ETL pipeline successfully streamlined the process of extracting, transforming, and loading diabetes data into a relational database. By improving data quality and structure, this approach enhances data analysis capabilities and supports better decision-making in healthcare analytics. Future improvements could involve automation, incorporating additional data sources, and implementing real-time ETL processes.

**How to Use**

**Install dependencies:** pip install pymongo pandas sqlalchemy psycopg2 matplotlib seaborn

Ensure MongoDB and PostgreSQL are running and configured properly.

Run the script in Jupyter Notebook or as a standalone Python script.

Verify data integrity in PostgreSQL using SQL queries.

For any suggestions or improvements, feel free to contribute!


