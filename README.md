# 🎥 Cinema Database Project

## 📌 Introduction
This project showcases the creation and management of a SQL Server database for a cinema. It includes database design, data insertion, execution of complex queries, and backup/restore operations. The project aims to demonstrate a wide range of SQL and database management capabilities, from data import to advanced analytics.

---

## 📁 Project Files Overview
The project consists of two main SQL files:

-   `insert_tables.sql`: This file contains the SQL scripts for creating the `Films` database and its various tables (`Directors`, `Customers`, `Genres`, `Movies`, `Views`). Additionally, it includes `INSERT` statements to populate these tables with initial data.
-   `Database_operations.sql`: This file contains SQL scripts for a wide array of database operations, including:
    * Bulk data import from CSV files.
    * Complex data update statements.
    * Advanced queries utilizing JOINs, Subqueries, and Window Functions.
    * Stored procedures for database backup and restore.

---

## 🛠 Tools & Technologies Used
-   **SQL Server Management Studio (SSMS)**: Development and management environment for SQL Server databases.
-   **SQL Server**: Relational Database Management System (RDBMS).
-   **SQL**: Structured Query Language for data management.

### Capabilities and Skills Demonstrated:
-   Database design and modeling.
-   Writing advanced SQL queries.
-   Data manipulation (INSERT, UPDATE).
-   Importing data from external formats (CSV).
-   Developing Stored Procedures.
-   Data backup and recovery strategies.
-   Troubleshooting and adjusting file paths.

---

## 📊 Database Structure and Usage

### Prerequisites
-   SQL Server Management Studio (SSMS) or any compatible SQL client.
-   SQL Server installed (e.g., SQL Server Express, Developer Edition).

### Steps to Set Up the Database

1.  **Create the Database and Tables:**
    * Open `insert_tables.sql` in SSMS.
    * Execute the entire script. This will create the `Films` database and all necessary tables, then populate them with initial data.

2.  **Perform Database Operations:**
    * Open `Database_operations.sql` in SSMS.
    * **Important Note:** Before running, you will need to **adjust the file paths** for the `BULK INSERT` command (for `views_data.csv`) and the `BACKUP DATABASE` and `RESTORE DATABASE` commands. Look for comments indicating where path changes are needed (e.g., `C:\\final_Project_sql\\views_data.csv` and `C:\\Users\\Public`).
    * Execute sections of the script as needed to perform updates, run queries, or manage backups.

---

## 📈 Key Operations Covered in `Database_operations.sql`

* **Data Import**: Demonstrates `BULK INSERT` from a CSV file.
* **Data Updates**: Examples of `UPDATE` statements to modify existing data based on specific conditions.
* **Advanced Queries**:
    * Use of `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN` to combine tables.
    * Use of `GROUP BY` and aggregate functions (`COUNT`, `SUM`, `AVG`) for data summarization.
    * Use of Subqueries for complex logic.
    * Use of Window Functions such as `ROW_NUMBER`, `RANK`, `DENSE_RANK`, `NTILE` for advanced data analysis.
* **Backup and Restore**: Stored procedures to create dated backups and restore the database from a backup file.

---

## 🔍 Key Insights and Applications

This project demonstrates how to build and maintain an efficient database system for a cinema. Through the operations presented, you can learn about:

* **Customer and Movie Management**: How to store and update details of customers, directors, genres, and movies.
* **Viewing Tracking**: Recording and analyzing customer viewing data for films.
* **Performance Analysis**: Advanced queries enabling the analysis of viewing trends, profitability (if data includes profit details), and customer behavior.
* **Data Resiliency**: The importance of backups and the ability to restore information in case of data loss.

This project serves as an excellent foundation for understanding relational database principles and their application in a SQL Server environment.
