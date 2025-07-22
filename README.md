# 🎥 Cinema Database Project

## 📌 Introduction
This project showcases the creation and management of a SQL Server database for a cinema. It involves robust database design, efficient data manipulation, execution of complex analytical queries, and the implementation of critical data management procedures like backup and restore. The primary goal is to demonstrate a comprehensive understanding of SQL and relational database principles, offering a solid foundation for data professionals.

---

## 📁 Project Files Overview
The project consists of two main SQL files, each serving a distinct purpose in the database lifecycle:

-   `insert_tables.sql`: This foundational script meticulously defines the schema for the `Films` database and its interconnected tables (`Directors`, `Customers`, `Genres`, `Movies`, `Views`). It includes `CREATE TABLE` statements with appropriate data types and constraints, followed by `INSERT` statements to populate these tables with initial, representative data, ensuring a ready-to-use dataset for analysis and operations.
-   `Database_operations.sql`: This file contains a suite of advanced SQL operations designed to demonstrate sophisticated database interactions:
    * **Data Ingestion**: Efficient `BULK INSERT` commands for importing large datasets (e.g., `views_data.csv`), showcasing data loading capabilities.
    * **Data Transformation & Integrity**: Complex `UPDATE` statements that reflect business logic and maintain data consistency across tables (e.g., updating customer watch counts, managing VIP benefits).
    * **Advanced Querying**: A rich collection of queries demonstrating:
        * Various `JOIN` types (`INNER`, `LEFT`, `RIGHT`) for data integration across multiple entities.
        * `Subqueries` for layered data retrieval and conditional logic.
        * Powerful `Window Functions` (`ROW_NUMBER`, `RANK`, `DENSE_RANK`, `NTILE`) for complex analytical tasks like ranking movies by income within genres or segmenting customers.
    * **Database Administration**: Implementation of `Stored Procedures` for automated and parameterized database backup and restore operations, highlighting critical data resiliency practices.

---

## 🛠 Tools & Technologies Used
-   **Microsoft SQL Server Management Studio (SSMS)**: Utilized for database development, administration, and query execution.
-   **Microsoft SQL Server**: The core Relational Database Management System (RDBMS) where the database is hosted and managed.
-   **SQL (Structured Query Language)**: The primary language used for all database interactions, from schema definition to advanced data analysis.

### Capabilities and Skills Demonstrated:
-   **Relational Database Design**: Implementation of a normalized schema (Directors, Customers, Genres, Movies, Views) to minimize redundancy and optimize data integrity.
-   **Data Manipulation Language (DML)**: Proficient use of `INSERT`, `UPDATE`, and `DELETE` (implied by update operations) statements.
-   **Data Definition Language (DDL)**: Comprehensive use of `CREATE DATABASE`, `CREATE TABLE`, `GO`, and `USE` commands.
-   **Performance Optimization (Implicit)**: Structured queries designed for efficiency and readability.
-   **Business Logic Implementation**: Translating business rules into SQL operations (e.g., VIP customer benefits, calculating watch counts).
-   **Procedural SQL**: Development and execution of `Stored Procedures` for repeatable tasks.
-   **Data Lifecycle Management**: Demonstrating essential backup and restore procedures for data governance and disaster recovery.

---

## 📊 Database Structure and Usage

### Prerequisites
-   SQL Server Management Studio (SSMS) or any compatible SQL client installed.
-   An instance of SQL Server (e.g., SQL Server Express, Developer Edition) accessible.

### Steps to Set Up the Database

1.  **Initialize Database and Tables:**
    * Open the `insert_tables.sql` file in SSMS.
    * Execute the entire script. This action will create the `Films` database, define all its necessary tables (e.g., Directors, Movies, Customers), and populate them with a foundational set of data.

2.  **Execute Database Operations:**
    * Open the `Database_operations.sql` file in SSMS.
    * **Crucial Note for Execution**: Before running, you *must* adjust the file paths specified within the `BULK INSERT` command (for `views_data.csv`) and the `BACKUP DATABASE`/`RESTORE DATABASE` commands. Look for inline comments (e.g., referencing `C:\\final_Project_sql\\views_data.csv` and `C:\\Users\\Public`) that indicate where these path modifications are required to match your local environment.
    * Execute sections of the script incrementally to observe data updates, execute various analytical queries, or perform database backup and restore routines.

---

## 📈 Key Operations Highlighted in `Database_operations.sql`

* **Efficient Data Ingestion**: Demonstration of `BULK INSERT` for rapid population of the `Views` table from external CSV data, a crucial skill for handling large datasets.
* **Intelligent Data Updates**: Examples of `UPDATE` statements that apply conditional logic (e.g., setting `NULL` for VIP customer benefits) and aggregate data to maintain referential integrity and consistency (e.g., updating `NumOfWatchedMovies` in the `Customers` table based on actual view counts).
* **Advanced Data Analysis**: A diverse set of queries showcasing the power of SQL for extracting deep insights:
    * **Relational Joins**: Integrating data across `Movies`, `Directors`, `Customers`, `Genres`, and `Views` to create comprehensive datasets.
    * **Data Aggregation**: Summarizing data using `GROUP BY` and aggregate functions (`COUNT`, `SUM`, `AVG`) to identify trends and key metrics.
    * **Complex Filtering with Subqueries**: Using nested queries to filter data based on results from another query, enabling sophisticated data segmentation.
    * **Analytical Ranking and Partitioning (Window Functions)**: Employing `ROW_NUMBER`, `RANK`, `DENSE_RANK`, and `NTILE` to perform partitioned analysis, such as ranking movies by income within each genre, or segmenting customers based on viewing habits.
* **Robust Database Maintenance**: Implementation of `Stored Procedures` for streamlined and automated:
    * **Dated Backups**: Creating database backups with dynamically generated filenames incorporating timestamps, essential for organized disaster recovery.
    * **Database Restore**: Procedures for restoring the database from a specified backup file, ensuring data recoverability.

---

## 🚀 Technical Highlights & Business Value
This project stands as a testament to practical SQL Server database management skills, offering significant value to a data-driven environment:

* **Foundation for Business Intelligence**: The well-structured database and advanced queries lay the groundwork for powerful reporting and Business Intelligence (BI) dashboards, enabling data-driven decision-making for cinema operations (e.g., identifying popular genres, optimizing movie schedules, personalizing customer experiences).
* **Data Integrity & Reliability**: Demonstrates an understanding of maintaining high data quality through controlled updates and robust backup/restore mechanisms, which are critical for operational continuity.
* **Scalability & Performance**: The design principles and use of efficient SQL constructs contribute to a scalable solution capable of handling growing data volumes.
* **Problem-Solving & Adaptability**: The necessity to adjust file paths for bulk inserts and backups highlights practical problem-solving skills in different deployment environments.
* **Comprehensive Skillset**: Showcases a full spectrum of database development and administration skills, from schema design and data population to complex querying and disaster preparedness, making it a valuable asset for roles involving data engineering, database administration, or data analysis.
