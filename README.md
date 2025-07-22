# Cinema Database Project

## Overview
This project involves the creation and management of a SQL Server database for a cinema. It includes tables for movies, directors, customers, genres, and views, along with various operations such as data insertion, updates, queries, and backup/restore procedures.

## Project Files
- `insert_tables.sql`: This file contains the SQL scripts to create the `Films` database and its tables (Directors, Customers, Genres, Movies, Views). It also includes `INSERT` statements to populate these tables with initial data.
- `Database_operations.sql`: This file contains SQL scripts for various database operations, including:
    - Bulk import from CSV.
    - Data update statements.
    - Complex queries with joins, subqueries, and window functions.
    - Stored procedures for database backup and restore.

## Database Setup and Usage

### Prerequisites
- SQL Server Management Studio (SSMS) or any compatible SQL client.
- SQL Server installed (e.g., SQL Server Express, Developer Edition).

### Steps to Set Up the Database

1.  **Create the Database and Tables:**
    * Open `insert_tables.sql` in SSMS.
    * Execute the entire script. This will create the `Films` database and all necessary tables, then populate them with initial data.

2.  **Perform Database Operations:**
    * Open `Database_operations.sql` in SSMS.
    * **Important Note:** Before running, you will need to **adjust the file paths** for the `BULK INSERT` command (for `views_data.csv`) and the `BACKUP DATABASE` and `RESTORE DATABASE` commands. Look for comments indicating where path changes are needed (e.g., `C:\\final_Project_sql\\views_data.csv` and `C:\\Users\\Public`).
    * Execute sections of the script as needed to perform updates, run queries, or manage backups.

### Key Operations Covered in `Database_operations.sql`

* **Data Import:** Demonstrates `BULK INSERT` from a CSV file.
* **Data Updates:** Examples of `UPDATE` statements to modify existing data based on specific conditions.
* **Advanced Queries:**
    * `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`
    * `GROUP BY` and aggregate functions (`COUNT`, `SUM`, `AVG`)
    * Subqueries
    * Window functions (`ROW_NUMBER`, `RANK`, `DENSE_RANK`, `NTILE`)
* **Backup and Restore:** Stored procedures to create dated backups and restore the database from a backup file.

## How to Upload to GitHub

1.  **Create a New Repository:**
    * Go to [GitHub](https://github.com/) and log in.
    * Click on the "New" button (or the "+" sign in the top right corner and select "New repository").
    * Give your repository a name (e.g., `Cinema-Database-Project`).
    * Add a brief description.
    * Choose whether it's public or private.
    * **Do NOT initialize with a README yet**, as we're creating our own.
    * Click "Create repository".

2.  **Initialize a Local Git Repository:**
    * Open your terminal or Git Bash.
    * Navigate to the folder where your `insert_tables.sql` and `Database_operations.sql` files are located.
    * Run `git init`

3.  **Add Your Files:**
    * Place the `README.md` file (the content above) into the same folder.
    * Run `git add .` (this stages all files in the current directory).

4.  **Commit Your Files:**
    * Run `git commit -m "Initial commit: Add cinema database project files and README"`

5.  **Link to Your GitHub Repository:**
    * On your GitHub repository page, you'll see instructions under "…or push an existing repository from the command line". Copy the `git remote add origin ...` line and paste it into your terminal and run it. It will look something like:
        `git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git`

6.  **Push Your Files to GitHub:**
    * Run `git push -u origin master` (or `main` if your default branch is `main`).

Now your project will be live on GitHub with a well-structured `README.md` file!
