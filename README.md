# 🎬 Cinema SQL Database Project

## 📌 Overview  
As a data analyst passionate about turning data into strategy, I built this full-scale **cinema database project** to simulate a real-world movie theater chain.

The project covers everything from **relational database design**, **data ingestion**, and **automated logic (via triggers & functions)** to **advanced analytics** and **insight generation** - all written in **pure SQL**.

🎯 The goal: Build a database that reveals **what drives revenue**, **how customers behave**, and **where business decisions can boost profitability**.

---

## 🎯 Project Objective  
To develop a complete SQL Server database that enables cinema management to make smarter decisions by answering questions like:

- Who are our most profitable customers?
- Which genres or actors bring in the most views and income?
- Which branches underperform — and what can we do about it?
- How do we increase customer retention with personalized offers?

The database supports both operational needs and future BI dashboard development.

---

## 🧱 Database Structure

The database is built on a relational schema (`Films`) with the following interconnected tables:

- 🎬 `Movies`: Includes movie name, director, main actor, genre, release year, and income  
- 🎭 `Genres`, 🎥 `Directors`, 👤 `MainActors`: Lookup/reference tables  
- 👥 `Customers`: Customer data, including favorites, watch count, and VIP status  
- 🏢 `Cinemas` & `Branches`: Cinema chain info with geolocation and facilities  
- 🍿 `Views`: Logs each transaction — what customer watched, where, and how

---

## 📂 Project Files

- `insert_tables.sql`  
  - Creates all tables and relationships  
  - Populates each table with realistic sample data

- `Database_operations.sql`  
  - 💾 **BULK INSERT** from external CSV  
  - 🔄 **UPDATE logic**: Automatically updates number of watched movies  
  - 🎯 **Triggers**: Update `NumOfWatchedMovies` and VIP status after insert  
  - ⭐ **Trigger-based VIP logic**: Adds new VIPs to a separate `vip_customers` table  
  - 🧮 **Functions**: Custom logic like calculating VIP eligibility  
  - ⚙️ **Stored Procedures**:  
    - Backup and restore routines  
    - Parameterized procedures for automation  
  - 📊 **Analytical queries**: Join-heavy, subqueries, aggregations, and ranking

---

## 🧠 Business Insights Uncovered

Based on the structure and queries in the project, here are key business insights that a cinema chain could apply in practice:

### 🔍 Key Insights:

1. **VIP automation enables targeted loyalty programs**  
   A trigger-based system identifies VIP customers based on their viewing activity. This can be used to send automatic rewards (e.g., free tickets, discounts), improving retention and lifetime value of high-engagement customers.

2. **High-income genres drive programming decisions**  
   Analyzing income by genre helps prioritize screenings of more profitable genres during high-demand periods — improving overall revenue efficiency.

3. **Branch-level profitability reveals where to invest — and where to optimize**  
   By comparing branches based on average income per view, total VIP share, and number of transactions, management can detect:
   - Top-performing locations to replicate
   - Underperforming ones to review staffing, scheduling, or marketing

4. **Top actors and directors boost ticket sales**  
   Using analytical ranking (window functions), we identify which actors/directors generate the highest revenue. This insight can guide:
   - Movie acquisition strategies
   - Marketing focus (e.g., promoting stars known to boost sales)

5. **Snack and drink data can uncover upsell potential**  
   With data on popcorn, drinks, and ice cream sales linked to hall type (VIP vs. regular), we can analyze:
   - Whether VIP viewers purchase more premium items
   - Which combos generate the highest profit margins
   This can help create targeted bundle offers to increase concessions revenue.

6. **Customer segmentation opens personalization opportunities**  
   By aggregating watch habits, spending patterns, and snack preferences, we can segment customers into personas (e.g., “family viewers”, “loyal action fans”, “weekend-only viewers”) and personalize promotions or recommendations accordingly.

7. **Retention risk detection via inactivity**  
   Customers who drop below a viewing frequency threshold (e.g., haven’t watched in 3+ months) can be flagged for re-engagement campaigns — minimizing churn.


---

## 🧪 SQL Capabilities Demonstrated

- ✅ **Relational Design** with proper normalization, constraints, and foreign keys  
- 📥 **BULK INSERT** for efficient data ingestion  
- 🧠 **Stored Procedures** for automation (e.g., `backup_database`, `restore_database`)  
- 🔁 **Triggers** for real-time logic updates (e.g., auto-VIP promotion after a new view)  
- 🔍 **Custom Scalar Functions** (e.g., check if a customer is eligible for VIP)  
- 🧩 **Joins & Aggregations**: Deep cross-table insights  
- 🧱 **Window Functions**:  
  - `RANK`, `DENSE_RANK`, `NTILE`, `ROW_NUMBER`  
  - Segmenting customers, ranking income by genre, etc.  
- 🧼 **Update logic** to preserve data integrity across interconnected tables

---

## 🛠 Tools Used

- **SQL Server Management Studio (SSMS)**  
- **Microsoft SQL Server** (tested on Developer Edition)  
- **SQL (DDL, DML, Procedural SQL)**

---

## 🚀 How to Run the Project

### Prerequisites:
- Microsoft SQL Server (Developer/Express)
- SSMS or compatible SQL client

### Setup Instructions:

1. Run `insert_tables.sql` to create the database and populate tables  
2. Open `Database_operations.sql` and:
   - Adjust file paths for `views_data.csv` and backups (see inline comments)  
   - Run queries and procedures step-by-step to see business logic in action

---

## 📈 Project Value & Use Cases

This project simulates a real-world cinema chain’s operational and analytical needs. Potential use cases include:

- 📊 BI Dashboards (Power BI, Tableau, Excel)  
- 🧠 Executive Reporting: Profit by region, genre, or customer segment  
- 🎯 Targeted Campaigns for VIPs and profitable customer segments  
- 🍿 Snack & upsell optimization based on behavior  
- 📍 Branch-level performance review

---

## 🙋‍♂️ About Me

I'm a data analyst driven by curiosity and business impact. I enjoy building complete systems that connect raw data to real decisions.  
This project was built in my spare time as part of my journey to master both **SQL development** and **strategic analytics**.

Feel free to explore the code — and connect with me if you're building something similar!
