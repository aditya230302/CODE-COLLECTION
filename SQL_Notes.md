# **Definitions**
- **Data**
  - A collection of information (Raw facts and figures). E.g. Numbers, test, images, etc.
- **SQL**
  - Structured query language (SQL) is a programming language for storing and processing information in a relational database.
  - Supports CSV, Excel, Commands.
- **Database**
  - A databse is an organised collection of structured information or data, typically stored electronically in a computer system.
  - A database is usually controlled by a database management system (DBMS).
- **DBMS**
  - A Database Management System (DBMS) is a software system that allows users to create, define, manipulate and manage databases. It provides a way for organizations to store, organize and retrieve large amounts of data quickly and efficiently in an organized manner.
  - E.g. MySQL, PostgreSQL, Oracle, MS SQL Server
- **RDBMS**
  - Relational Database Management System, is a type of database management system (DBMS) that organizes data into tables with rows and columns, where relationships between tables are defined using common attributes.
  - It uses the relational model of data, which structures data into tables that can be linked together, making it efficient for storing and retrieving related information.
  - RDBMS uses SQL (Structured Query Language) to manage and query the data.
  - In a database different tables should not have the same name.
  - Columns are fields (y-axis).
  - Rows are records (x-axis).
- **Primary Key**
  - Not Null + Unique value
- **Foreign Key**
  - Not Null + Unique value related to primary key in another table
- **Candidate Key**
  - Have all the pre-requists of primary key, but we don't consider it as primary key
---

## **Types of Data**
**1. Structured Data** : Data that is formated properly and can be easily interpreted by anyone. It is supported by DBMS/RDBMS.
**2. Semi-Structured Data** : Partially structured data. E.g. emails, json files, xml/html files, csv files.
**3. Unstructured Data** : Unformated Data. E.g. audio, video, images, etc.

---
## **Types of Databases**
- **Tables**
- **RDBMS**
  - Any RDBMS must support the following relations
    - One to One i.e. 1 : 1
    - One to Many i.e. 1 : Many
    - Many to Many i.e. Many : Many
- **No SQL Database**
  - Stores data that can't be stored in tables. E.g. images, emails, social media posts, steaming, chat messages, charts, etc.
  - E.g. MongoDB, CouchDB, GraphDB, ApacheDB
---
# **Data Warehouse (DWH)**
- A data warehouse is a centralized repository designed for storing large amounts of data from various sources, enabling organizations to perform in-depth analysis and generate reports for better decision-making
- Only the data which is structured/formated is stored in Data warehouse.
- Data Warehouse is an appliance for storing and analyzing data, and reporting.
- It is designed for query and analysis.
- It usually contains historical data derived from transaction data or other sources.

## **Real - Time Data Warehouse**
- Server rooms
- DWH is like an on-premise server, its safer than working with thirdparty servers.

## **Data Warehouse Architecture**

![image](https://github.com/user-attachments/assets/19ac9003-da2d-4262-9bb3-179cf4b15dd5)

## **Data Warhousing Process**
1. **Data Cleaning:** It includes filling in missing values, smoothing noisy data removing outliers and resolving incosistencies.
2. **Data infegeration:** It includes infegeration of multiple database, data cubes and files.
3. **Data transformation:** Converts data fron host format to warehouse format
4. **Data loading:** Sort, summarize, consolidate, compute, views, check integrity
5. **Data refreshing:** Propagates the updates from data sources to the warehouse.

## **Characteristics Of Datawarehouse**
1. **Subject ariented:** It can be used to analyze a particular subject area
2. **Integerated:** It integerates data from. multiple data sources.
3. **Time variant:** Historical data is kept in a data warehouse.
4. **Non volatile:** Once data is in the warehouse, it will not changes

## **Components of data warehouse:**
- **Central Database:** A database serves as the foundation of your data warehouse
- **Data Integeration:** Data is pulled from many Source system and modified.
- **Meta Data:** It specifies the source, usage, values and other features of the data
- **Access Tools:** It allows users to interact with data in your data warehouse. E.g. OLAP tools.

## **Applications of Data Warehouse**
- Services, Banking, INsurance, Finance, Retailing, Education, Manufacturing, Healthcare

---
# **Data Mart**
- Subsets of DWH, they are comprised completely of only specific departments/category/business units.
- It exists independently without being integerated into a data warehouse.
- they provide quick and easy access to data for individual category, eliminating the need to search through the entire data warehouse.

## **Uses of Data Mart**
- Indentifying trends and patterns
- Making informed decisions
- improving the operational efficiency

## **Benefits of Data Mart**
- Improved access of data
- Faster analysis
- Reduced Costs

## **Data Mart Architecture**

![image](https://github.com/user-attachments/assets/6e8982c5-de15-42d1-bda9-b7378d186a25)

---
# **Data Mart vs Data Warehouse**

| Feature             | **Data Mart**                                                                        | **Data Warehouse**                                                                          |
| ------------------- | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------- |
| **Main Definition** | A **subset** of a Data Warehouse. Focused on a specific business line or department. | A **central repository** of data collected from various departments across an organization. |
| **Size**            | Typically **less than 100 GB**                                                       | Usually **more than 100 GB**                                                                |
| **Scope**           | Covers a **single department or business unit**                                      | Covers the **entire organization**                                                          |
| **Time to Build**   | Takes **a few weeks to a few months**                                                | Takes **many months or even years**                                                         |
| **Organization**    | Managed by **individual departments**                                                | Managed by **central IT or data team**                                                      |

---
# **DBMS vs Data Warehouse**

| **DBMS**   | **Data Warehouse** |
| ---------- | ------------------ |
| It is Transaction oriented | It is Subject oriented |
| Contains detailed data | Contains historic data |
| It captures data | It analyzes data |
| Application Oriented | Subject Oriented |

---
# **OLAP (Online Analytical Processing)**
- OLAP is used for data preparation in data data warehouses.
- It is a computing method that allows users to easily and selectively extract data.
- It is used to query data in order to analyze it from different point of views.
- OLAP business intelligence often helps in trend analysis, financial reporting, sales forecasting, budgeting and other planning processes.
- OLAP helps in making data mart.
- OLAP maintains data in a cubical structure.
- Examples of OLAP Tools: IBM Cognos, Oracle OLAP, Tableau, Domo, Sisense, and Reveal. 

![image](https://github.com/user-attachments/assets/a6ec80c3-2a91-41dc-a765-b205012536a6)

---
# **OLTP (Online Transactional Processing)**
- It facilitates and manageges transaction oriented applications (typically involving data entry and retrieval).
- OLTP enabels large number od database transactions(insertion, deletion or query of data in a DB) made by large number of people over the internet.
- OLTP system drives many of the financial transactions made everyday including online transaction, ATM transaction, E-commerce and in-store purchase.
- Examples include:
  - Database Management Systems (DBMS): PostgreSQL, MySQL, Oracle Database, Microsoft SQL Server, CockroachDB, IBM Db2, MongoDB. 
  - Applications: ATMs, online banking, e-commerce, ticketing systems, and recordkeeping systems like health records and inventory control.

![image](https://github.com/user-attachments/assets/a2867627-a7eb-4674-9bb1-1f0e3c8f12f3)

---
# **OLTP vs OLAP**

| Feature             | **OLTP**                                                | **OLAP**                                                    |
| ------------------- | ------------------------------------------------------- | ----------------------------------------------------------- |
| **Full Form**       | Online Transaction Processing                           | Online Analytical Processing                                |
| **Purpose**         | Handles **day-to-day transactions**                     | Used for **data analysis and decision making**              |
| **Users**           | **Clerks, cashiers, DBAs**                              | **Analysts, managers, executives**                          |
| **Operations**      | **Insert, Update, Delete** (short, atomic transactions) | **Read-heavy operations** like complex queries and analysis |
| **Data Volume**     | Processes **large numbers of small transactions**       | Works with **fewer but complex and large queries**          |
| **Response Time**   | **Milliseconds to seconds**                             | **Seconds to minutes (can be longer)**                      |
| **Database Design** | **Highly normalized** (to reduce redundancy)            | **De-normalized** (for faster read access and joins)        |
| **Data Source**     | Real-time **current data**                              | Historical **aggregated data**                              |
| **Examples**        | Banking systems, e-commerce, retail POS systems         | Data warehouses, business reporting systems                 |


## **OLTP and OLAP working together**
- user will give queries to the data warehouse/data mart through OLTP Database for analytical pr=urpose and the query will go to OLAP cube to acces data.

![image](https://github.com/user-attachments/assets/87bd5882-bfab-41ad-a414-bfd839e544b1)

---
# **Multidimensioanl Data Model**
- The multidimensional datamodel is used to store the data in the form of **Data cubes**.
- A data cube allows data to be viewed in multiple dimensions.
- Here the dimensions are the entities with respect to which an organisation keeps the records.
- It provides machanism to store data and a way for business analysis.
- **Dimensions** and **Facts** are two components of multidimensional data model.
- **Dimensions** : are the text attributes to analyze data
- **Facts** : are the numeric volume to analyze business.
- It helps to provide fast and accurate data-related answers to complex business queries.

![image](https://github.com/user-attachments/assets/2b0a9d40-558d-47f1-9c40-7fbc9eb96f8e)

---
# **Schema for Multidimensional Model**
## **1. Star Schema**
- It is the simplest data warhouse schema because it resembles a star.
- In star every Dimensional table is connected to the Fact table using primary key(dimensional table) to foreign key(Fact table) relationship.

![image](https://github.com/user-attachments/assets/eeb69298-8476-412b-afa4-5194aea7f0b6)

## **2. Snowflake Schema**
- In Snowflake schema dimensional tables are connected to other dimensional tables.
- It is more complex than Star Schema.

![image](https://github.com/user-attachments/assets/f047ed57-9a8d-4e67-9a81-54e85dcbd673)

## **3. Fact Constellation Schema**
- This schema has multiple fact tables, which dhare many fimensional tables.
- this type of schema can be viewed as a star and snowflake schema, hence it is also called **Galaxy Schema** or Fact Constellation Schema.
- This main disadvantage of this shema is that it has more complex design.

![image](https://github.com/user-attachments/assets/470d0fa6-673c-49eb-b9c3-45ab997c16f9)

---
# **SQL Query Execution Order**
| **Step** | **Clause**       | **Description**                                                         |
| -------- | ---------------- | ----------------------------------------------------------------------- |
| 1        | `FROM`           | Identifies source tables and joins them if needed                       |
| 2        | `WHERE`          | Filters rows before grouping                                            |
| 3        | `GROUP BY`       | Groups rows based on specified columns                                  |
| 4        | `HAVING`         | Filters groups (after aggregation)                                      |
| 5        | `SELECT`         | Selects columns or expressions to return                                |
| 6        | `DISTINCT`       | Removes duplicate rows (if specified)                                   |
| 7        | `ORDER BY`       | Sorts the result set                                                    |
| 8        | `LIMIT / OFFSET` | Limits the number of rows returned (if used, e.g., in MySQL/PostgreSQL) |
---
# **SQL Command Types**

## **1. DDL (Data Definition Language)**
- Used to define and manage database structure (tables, schemas, etc.)
- **CREATE** : used to create new tables/databases/views/stored procedures/functions/triggers/indexes
- **ALTER** : used to modify design of a table (ADD/REMOVE/MODIFY)
- **DROP** : Remove Table/databases/views/stored procedures/functions/triggers/indexes
- **TRUNCATE** : Remove all rows from a table without logging individual row deletions. Faster than DELETE.

## **2. DML (Data Manipulation Language)**
- Used to manipulate data in tables.
- **INSERT** : Inserting new records
- **UPDATE** : Modifying existing records
- **DELETE** : Delete specific rows from a table (with WHERE clause).
  
## **3. TCL (Transaction Control Language)**
- Used to manage transactions (group of SQL operations).
- **BEGIN TRANSACTION** : Starts a new transaction block.
- **COMMIT** : Permanently saves all changes made during the transaction.
- **ROLLBACK** : 	Undoes changes since the last COMMIT.
- **SAVE** : 	Sets a point in a transaction to which you can roll back to later.

## **4. DCL (Data Control Language)**
- Used to control access and permissions to data in the database.
- **GRANT** : Give privileges/access to users/roles (e.g., SELECT, INSERT, EXECUTE).
- **REVOKE** : Remove access/privileges granted to users/roles.
```sql
-- Create a new user (assumes login already exists)
CREATE USER John FOR LOGIN JohnLogin;

-- Grant SELECT permission on the Employees table to John
GRANT SELECT ON Employees TO John;

-- Revoke SELECT permission from John
REVOKE SELECT ON Employees FROM John;
```
## **5. DQL (Data Query Language)**
- Used to query and fetch data from the database.
- **SELECT** : 	Retrieves data from one or more tables/views. It's the only DQL command.

---
Every table or any object created in DB will have schema called as `**DBO.<OBJECT_Name>**`
- example of objects are : Database object, tables, views,index,stored procedures, functions, etc.
---
# **SELECT**
- Used to get data from table.
- Syntax :
```sql
SELECT <column names with commas> from <Table name>
```
- Example :
```Sql
-- " * " is used to fetch all records
SELECT *
FROM Employee_Table

Select Emp_name, Emp_ID
from Employee_Table
```
---
# **SQL Clauses**
| **Clause** | **Purpose**                                                            |
| ---------- | ---------------------------------------------------------------------- |
| `FROM`     | Specifies the **table** to retrieve data from.                         |
| `WHERE`    | Filters rows **before** grouping or selection.                         |
| `GROUP BY` | Groups rows that have the same values in specified columns.            |
| `HAVING`   | Filters **groups** after `GROUP BY` (like `WHERE` but for aggregates). |
| `ORDER BY` | Sorts the result set by one or more columns.                           |

## **WHERE CLause**
- Filters rows **before** grouping or selection
- written always after table name only
- if there are multiple conditions then operators are used
- Syntax :
```Sql
SELECT <column name>
FROM <Table>
WHERE <Condition>
```
- Example :
```sql
SELECT * FROM Employee_Table WHERE DeptNo = 10
SELECT * FROM Employee_Table WHERE Job = 'Clerk' -- string is mentioned in ' '
```
---
# **Operators**
- `IN`, `NOT IN` : 
