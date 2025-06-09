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
- **1. Structured Data** : Data that is formated properly and can be easily interpreted by anyone. It is supported by DBMS/RDBMS.
- **2. Semi-Structured Data** : Partially structured data. E.g. emails, json files, xml/html files, csv files.
- **3. Unstructured Data** : Unformated Data. E.g. audio, video, images, etc.

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

## **FROM Clause**
- The `FROM` clause specifies the **table(s)** from which to retrieve data.

### ✅ Key Points:
* Always follows the `SELECT` statement.
* Can include **single or multiple tables** (joins).
* Acts as the **starting point** for data retrieval.

### 🧾 Syntax:
```sql
SELECT <column_name>
FROM <table_name>;
```

### 📌 Examples:
```sql
-- Select all columns from Employee_Table
SELECT * 
FROM Employee_Table;

-- Select specific columns from a table
SELECT EmpName, Salary 
FROM Employee_Table;
```

## **WHERE Clause**
- The `WHERE` clause is used to **filter rows** based on a condition **before** any grouping or aggregation happens.

### ✅ Key Points:
* Always written **after the `FROM` clause** and **before** `GROUP BY`, `HAVING`, or `ORDER BY`.
* Used to filter individual rows before aggregation.
* Multiple conditions can be combined using logical operators like `AND`, `OR`, and `NOT`.
* For string comparisons, values must be enclosed in single quotes `' '`.

### 🧾 Syntax:
```sql
SELECT <column_name>
FROM <table_name>
WHERE <condition>;
```

### 📌 Examples:
```sql
-- Select all rows where department number is 10
SELECT * 
FROM Employee_Table 
WHERE DeptNo = 10;

-- Select all employees whose job is 'Clerk'
SELECT * 
FROM Employee_Table 
WHERE Job = 'Clerk';
```

## **GROUP BY Clause**
- The `GROUP BY` clause is used to **group rows** that have the same values in specified columns, typically used with **aggregate functions**.
- used to prepare summary report in dashboards/analysis.

### ✅ Key Points:
* Comes **after `WHERE`** and **before `HAVING`**.
* Must include all non-aggregated columns in the `SELECT` list.
* Enables use of functions like `COUNT()`, `SUM()`, `AVG()`, `MAX()`, `MIN()`.

### 🧾 Syntax:
```sql
SELECT <column>, AGG_FUNCTION(<column>)
FROM <table>
WHERE <condition>
GROUP BY <column>;
```

### 📌 Examples:
```sql
-- Get total salary by department
SELECT DeptNo, SUM(Salary) 
FROM Employee_Table 
GROUP BY DeptNo;

-- Count employees in each job role
SELECT Job, COUNT(*) 
FROM Employee_Table 
GROUP BY Job;
```

## **HAVING Clause**
- The `HAVING` clause is used to **filter groups** after `GROUP BY` has been applied. It works like `WHERE`, but **for aggregated data**.

### ✅ Key Points:
* Always used **after `GROUP BY`**.
* Cannot be used without `GROUP BY` when filtering aggregates.
* Supports aggregate functions.

### 🧾 Syntax:
```sql
SELECT <column>, AGG_FUNCTION(<column>)
FROM <table>
GROUP BY <column>
HAVING <aggregate_condition>;
```

### 📌 Examples:
```sql
-- Show departments with total salary greater than 50000
SELECT DeptNo, SUM(Salary) 
FROM Employee_Table 
GROUP BY DeptNo
HAVING SUM(Salary) > 50000;

-- Show jobs with more than 3 employees
SELECT Job, COUNT(*) 
FROM Employee_Table 
GROUP BY Job
HAVING COUNT(*) > 3;
```

## **ORDER BY Clause**
- The `ORDER BY` clause is used to **sort** the result set by one or more columns.

### ✅ Key Points:
* Always appears at the **end** of the query.
* Default sorting is **ascending (`ASC`)**, descending order is specified using **`DESC`**.
* Can sort by column name or **column position** (index in the SELECT list).

### 🧾 Syntax:
```sql
SELECT <columns>
FROM <table>
ORDER BY <column> [ASC|DESC];
```

### 📌 Examples:
```sql
-- Sort employees by salary in ascending order
SELECT EmpName, Salary 
FROM Employee_Table 
ORDER BY Salary;

-- Sort employees by salary in descending order
SELECT EmpName, Salary 
FROM Employee_Table 
ORDER BY Salary DESC;

-- Sort by multiple columns
SELECT EmpName, DeptNo, Salary 
FROM Employee_Table 
ORDER BY DeptNo ASC, Salary DESC;
```

---

# **SQL Operators**
- SQL operators are used in `WHERE`, `HAVING`, and other clauses to filter or manipulate data. They are categorized into the following types:

## 🧮 **1. Comparison Operators**

| **Operator** | **Description**             | **Example**                      |
| ------------ | --------------------------- | -------------------------------- |
| `=`          | Equal to                    | `Salary = 50000`                 |
| `!=` or `<>` | Not equal to                | `DeptNo != 10`                   |
| `>`          | Greater than                | `Salary > 60000`                 |
| `<`          | Less than                   | `Salary < 30000`                 |
| `>=`         | Greater than or equal to    | `Experience >= 5`                |
| `<=`         | Less than or equal to       | `Age <= 40`                      |
| `BETWEEN`,`NOT BETWEEN`| Between a range (inclusive) | `Salary BETWEEN 30000 AND 60000` |
| `LIKE`,`NOT LIKE`      | Pattern matching            | `Name LIKE 'A%'`                |
| `IN`,`NOT IN`| When we want to filter `OR` condition or multiple values in 1 column | `DeptNo IN (10, 20, 30)`         |
| `IS NULL`,`IS NOT NULL`    | Checks if the value is NULL | `Manager_ID IS NULL`             |

- 0 is a value, NULL means there is no value
- for matching strings we can also use lowercase
- `%` in string means 'n' characters at that place, e.g. `A%` can be 'Adi', 'Abhinav', etc. and `%A` can be 'Vandana', 'Sharma', 'data',etc.
- `%O%` it contains 'O'
- `S%T` it starts with 's' and ends with 't'
- `_` mean 1 single charachter.
- `____` (i.e. 4 times `_`) means 4 characters, e.g. `_O__` means length is 4 and 2nd charchter is 'O'
  
## 🧠 **2. Logical Operators**

| **Operator** | **Description**                       | **Example**                     |
| ------------ | ------------------------------------- | ------------------------------- |
| `AND`        | True if **both** conditions are true  | `DeptNo = 10 AND Job = 'Clerk'` |
| `OR`         | True if **any one** condition is true | `DeptNo = 10 OR DeptNo = 20`    |
| `NOT`        | Negates a condition                   | `NOT (Job = 'Manager')`         |

## 🧪 **3. Arithmetic Operators**

| **Operator** | **Description**                | **Example**                                 |
| ------------ | ------------------------------ | ------------------------------------------- |
| `+`          | Addition                       | `Salary + Bonus`                            |
| `-`          | Subtraction                    | `Salary - Deduction`                        |
| `*`          | Multiplication                 | `Salary * 0.1`                              |
| `/`          | Division                       | `Salary / 12`                               |
| `%`          | Modulus (remainder) *(varies)* | `Salary % 1000` *(may not work in all DBs)* |

## 🔁 **4. Assignment Operator (Used in `UPDATE`)**

| **Operator** | **Description** | **Example**                          |
| ------------ | --------------- | ------------------------------------ |
| `=`          | Assigns a value | `UPDATE Employee SET Salary = 50000` |

## 🔍 **5. Pattern Matching Operators (Used with `LIKE`)**

| **Symbol** | **Description**         | **Example**                      |
| ---------- | ----------------------- | -------------------------------- |
| `%`        | Zero or more characters | `Name LIKE 'A%'` (starts with A) |
| `_`        | Exactly one character   | `Name LIKE '_a%'`                |

## 📝 Example Query Using Multiple Operators:

```sql
SELECT EmpName, Salary, DeptNo
FROM Employee_Table
WHERE Salary > 30000 AND DeptNo IN (10, 20)
ORDER BY Salary DESC;
```

---

# **SQL Aggregation Functions**
- Aggregation (or aggregate) functions perform **calculations on multiple rows** and return a **single summary value**. They are commonly used with `GROUP BY` and `HAVING`.
- They can't be used in where clause because where clause works before aggregation takes place.
- `SUM`, `AVG`, `MAX`, `MIN`, `COUNT`

## 🔢 **1. COUNT()**
- Returns the **number of rows** that match the condition.

### ✅ Syntax:
```sql
SELECT COUNT(*) FROM <table>;
SELECT COUNT(column_name) FROM <table>;
```

### 📌 Examples:
```sql
-- Count all rows in the table
SELECT COUNT(*) FROM Employee_Table;

-- Count non-null job titles
SELECT COUNT(Job) FROM Employee_Table;
```

## 💰 **2. SUM()**
- Returns the **total sum** of a numeric column.

### ✅ Syntax:
```sql
SELECT SUM(column_name) FROM <table>;
```

### 📌 Example:
```sql
-- Total salary of all employees
SELECT SUM(Salary) FROM Employee_Table;
```

## 📊 **3. AVG()**
- Returns the **average value** of a numeric column.

### ✅ Syntax:
```sql
SELECT AVG(column_name) FROM <table>;
```

### 📌 Example:
```sql
-- Average salary of employees
SELECT AVG(Salary) FROM Employee_Table;
```

## 📈 **4. MAX()**
- Returns the **maximum value** in a column.

### ✅ Syntax:
```sql
SELECT MAX(column_name) FROM <table>;
```

### 📌 Example:
```sql
-- Highest salary among employees
SELECT MAX(Salary) FROM Employee_Table;
```

## 📉 **5. MIN()**
- Returns the **minimum value** in a column.

### ✅ Syntax:
```sql
SELECT MIN(column_name) FROM <table>;
```

### 📌 Example:
```sql
-- Lowest salary among employees
SELECT MIN(Salary) FROM Employee_Table;
```

## 🧠 Aggregation with GROUP BY

You can combine these functions with `GROUP BY` to summarize data by categories.

### 📌 Example:
```sql
-- Total salary by department
SELECT DeptNo, SUM(Salary)
FROM Employee_Table
GROUP BY DeptNo;

-- Count of employees in each job role
SELECT Job, COUNT(*) 
FROM Employee_Table
GROUP BY Job;
```
## **ROLLUP function**
- it extends the functionality of group by.
- adds a row to the group by output.
- when applied on 1 column only adds `grand total` i.e `1 row`
- when applied on more than 1 column adds `grand total` according to first column and `subtotals` according to 2nd column (and so on for further columns)

### 🧾 Syntax:
```sql
group by Rollup(<col name>) -- must be in paranthesis
```

## **COALESCE function**
- it replaces null value in the specified column with the specified value

  ### 🧾 Syntax:
```sql
select COALESCE(<col name>, <value>) as <col name>,
from table
```

### 📌 Example:
```sql
-- ADD another row with null as index and null values as data which will be replaced by 'Grand Total' due to colaesce
SELECT COALESCE(REGION, 'GRAND TOTAL') AS REGION
FROM SUM(SALES) AS 'TOTAL SALES' -- USE ' ' FOR SPACE OR SPECIAL CHARACTERS
FROM SALESORDER
GROUP BY ROLLUP(REGION)
```

---

# **JOINS**
- Basically used to get information from multiple tables in 1 select statement.
- The tables must have a common column to join them.
- When we use `Join` then `Inner Join` is applied by default.

## **Types of joins**
| **Join Type** | **Returns**                                                                     |
| ------------- | ------------------------------------------------------------------------------- |
| `INNER JOIN`  | Only matching rows from both tables.                                            |
| `LEFT JOIN`   | All rows from the left table + matching rows from the right (NULL if no match). |
| `RIGHT JOIN`  | All rows from the right table + matching rows from the left (NULL if no match). |
| `FULL JOIN`   | All rows from both tables (NULLs where there’s no match).                       |

## **1. INNER JOIN**
- Returns only the **matching rows** from both tables.

### 🧾 Syntax:
```sql
SELECT a.column1, b.column2
FROM TableA a
INNER JOIN TableB b
ON a.common_column = b.common_column;
```

### 📌 Example:
```sql
SELECT E.EmpName, D.DeptName
FROM Employee E  
INNER JOIN Department D
ON E.DeptID = D.DeptID;
-- giving alias to tables make it easier to work with them when we have to write larger queries
-- an alias is limited to one script only
```
> ✅ Only employees who belong to a valid department will be shown.

## **2. LEFT JOIN (LEFT OUTER JOIN)**
- Returns **all rows from the left table** and **matched rows from the right**. If no match, NULLs are returned for the right table.

### 🧾 Syntax:
```sql
SELECT a.column1, b.column2
FROM TableA a
LEFT JOIN TableB b
ON a.common_column = b.common_column;
```

### 📌 Example:
```sql
SELECT E.EmpName, D.DeptName
FROM Employee E
LEFT JOIN Department D
ON E.DeptID = D.DeptID;
```
> ✅ Includes employees even if they don't belong to any department.

## **3. RIGHT JOIN (RIGHT OUTER JOIN)**
- Returns **all rows from the right table** and **matched rows from the left**. If no match, NULLs are returned for the left table.

### 🧾 Syntax:
```sql
SELECT a.column1, b.column2
FROM TableA a
RIGHT JOIN TableB b
ON a.common_column = b.common_column;
```

### 📌 Example:
```sql
SELECT E.EmpName, D.DeptName
FROM Employee E
RIGHT JOIN Department D
ON E.DeptID = D.DeptID;
```
> ✅ Includes all departments even if they have no employees.

## **4. FULL JOIN (FULL OUTER JOIN)**
- Returns **all rows from both tables**. If there's no match, NULLs are shown for non-matching sides.

### 🧾 Syntax:
```sql
SELECT a.column1, b.column2
FROM TableA a
FULL JOIN TableB b
ON a.common_column = b.common_column;
```

### 📌 Example:
```sql
SELECT E.EmpName, D.DeptName
FROM Employee E
FULL OUTER JOIN Department D
ON E.DeptID = D.DeptID;
```
> ✅ Includes all employees and all departments — even unmatched ones.

## **How to Join Multiple Tables**
```sql
SELECT * FROM EMP A
LEFT JOIN DEPT B
ON A.EMPID = B.EMPID
INNER JOIN PRODUCT P
ON P.DEPTNO = B.DEPTNO
```
---
# **SQL SET OPERATORS**
## **UNION**

## **UNION ALL**

## **INTERSECT**

## **EXCEPT**

---
# **SQL Data Types**

| **Data Type**            | **Description**                                           | **Example**            |
| ------------------------ | --------------------------------------------------------- | ---------------------- |
| `VARCHAR(n)`             | Variable-length **text**, up to **n characters**          | `EmpName VARCHAR(50)`  |
| `CHAR(n)`                | Fixed-length **text**, always stores **n characters**     | `Gender CHAR(1)`       |
| `TEXT`                   | Long variable-length text (non-indexed in many databases) | `Comments TEXT`        |
| `INT` / `INTEGER`        | Whole numbers (positive or negative)                      | `Age INT`              |
| `SMALLINT`               | Smaller-range whole numbers                               | `Rating SMALLINT`      |
| `BIGINT`                 | Very large whole numbers                                  | `Population BIGINT`    |
| `DECIMAL(p,s)`           | Exact numeric with precision `p` and `s` no. of decimals  | `Salary DECIMAL(10,2)` |
| `NUMERIC(p,s)`           | Same as `DECIMAL` (standard SQL), if s not mentioned then no decimals| `Price NUMERIC(8,2)`   |
| `FLOAT`                  | Approximate floating-point number                         | `Temperature FLOAT`    |
| `REAL` / `DOUBLE`        | More precision than `FLOAT`                               | `Longitude DOUBLE`     |
| `BOOLEAN`                | Logical TRUE or FALSE                                     | `IsActive BOOLEAN`     |
| `DATE`                   | Stores a calendar date (YYYY-MM-DD)                       | `BirthDate DATE`       |
| `TIME`                   | Stores time (HH\:MM\:SS)                                  | `LoginTime TIME`       |
| `DATETIME` / `TIMESTAMP` | Stores both date and time                                 | `CreatedAt DATETIME`   |
| `BLOB`                   | Binary Large Object (used for images, audio, etc.)        | `Photo BLOB`           |
| `NVARCHAR(n)`                   | Variable-length **Unicode** text (for multi-language support)                  | `CityName NVARCHAR(100)`                |
| `NCHAR(n)`                      | Fixed-length **Unicode** text                                                  | `Language NCHAR(2)`                     |
| `ENUM('a','b',...)`             | A string object with a predefined set of values (MySQL specific)               | `Gender ENUM('Male', 'Female')`         |
| `SET('a','b',...)`              | A string object that can store **multiple** predefined values (MySQL specific) | `Hobbies SET('Music','Sports','Books')` |
| `JSON`                          | Stores JSON-formatted data (MySQL/PostgreSQL)                                  | `Preferences JSON`                      |
| `XML`                           | Stores XML data (used in SQL Server)                                           | `ConfigData XML`                        |
| `YEAR`                          | Stores a year in 2-digit or 4-digit format (MySQL-specific)                    | `JoinYear YEAR`                         |


### 📝 Notes:
* Use `VARCHAR` for **names, emails, addresses** etc.
* Use `INT`, `DECIMAL`, or `FLOAT` for **numeric data**.
* Use `DATE`, `TIME`, or `DATETIME` for **temporal data**.
* Choose data types carefully to **optimize performance and storage**.

---

# **DDL Commands ( Data Definition Language)**
- Used to define and manage database structure (tables, schemas, etc.)
- **CREATE** : used to create new tables/databases/views/stored procedures/functions/triggers/indexes
- **ALTER** : used to modify design of a table (ADD/REMOVE/MODIFY)
- **DROP** : Remove Table/databases/views/stored procedures/functions/triggers/indexes
- **TRUNCATE** : Remove all rows from a table without logging individual row deletions. Faster than DELETE.

## **CREATE : To Create a Table**
### 🧾 Syntax:
```sql
CREATE TABLE <TABLE NAME> (
                            <COL NAME>  <DATA TYPE>,
                            <COL NAME>  <DATA TYPE>,
                            <COL NAME>  <DATA TYPE>,
                            ...
                          )
```

### 📌 Example:
```sql
CREATE TABLE EMP_001
(
EMPID  VARCHAR(50)  NOT NULL, -- NOT NULL IS A CONTRAINT
ENAME  VARCHAR(100),
SAL    NUMERIC(10,2),
DOJ    DATE,
DNAME  VARCHAR(50)
)
```
- To see table description :
```sql
SP_HELP <TABLE NAME>  -- SP stands for stored procedure
```
- A stored procedure is a group of SQL statements that are stored in a database and can be executed as a single unit

### **What Can `CREATE` Be Used For in SQL?**

| **Statement**                 | **Purpose**                                                                   |
| ----------------------------- | ----------------------------------------------------------------------------- |
| `CREATE DATABASE`             | Creates a new database                                                        |
| `CREATE TABLE`                | Creates a new table with specified columns and data types                     |
| `CREATE VIEW`                 | Creates a virtual table (view) based on a SELECT query                        |
| `CREATE INDEX`                | Creates an index on one or more columns to improve query performance          |
| `CREATE UNIQUE INDEX`         | Creates an index that ensures all values in the column(s) are unique          |
| `CREATE SCHEMA`               | Creates a new schema (logical container for database objects)                 |
| `CREATE PROCEDURE`            | Defines a stored procedure (set of SQL statements that can be reused)         |
| `CREATE FUNCTION`             | Defines a user-defined function that returns a value                          |
| `CREATE TRIGGER`              | Creates a trigger that runs automatically on specified table events           |
| `CREATE ROLE`                 | Creates a database role for managing permissions                              |
| `CREATE USER`                 | Creates a new database user (depends on DBMS and user permissions)            |
| `CREATE TYPE`                 | Creates a user-defined data type (used in SQL Server, PostgreSQL, etc.)       |
| `CREATE SEQUENCE`             | Creates a sequence object for generating numeric values (like auto-increment) |
| `CREATE SYNONYM` (SQL Server) | Creates an alias or alternative name for another database object              |

#### 📌 Examples

##### 1. Create a Database
```sql
CREATE DATABASE SchoolDB;
```
##### 2. Create a Table
```sql
CREATE TABLE Students (
  StudentID INT PRIMARY KEY,
  Name VARCHAR(100),
  Age INT,
  EnrolledDate DATE
);
```
##### 3. Create a View
```sql
CREATE VIEW ActiveStudents AS
SELECT Name, Age FROM Students WHERE EnrolledDate >= '2023-01-01';
```
##### 4. Create an Index
```sql
CREATE INDEX idx_name ON Students(Name);
```
##### 5. Create a Stored Procedure
```sql
CREATE PROCEDURE GetStudentByID @ID INT
AS
BEGIN
  SELECT * FROM Students WHERE StudentID = @ID;
END;
```

## **DROP : To Remove a Table**
### 🧾 Syntax:
```sql
DROP TABLE <TABLE NAME>
```

### 📌 Example:
```sql
DROP TABLE EMP_OO1
```

## **Add New Columns to the Table**
### 🧾 Syntax:
```sql
ALTER TABLE <TABLE NAME> ADD <COL NAME> <DATA TYPE>
```

### 📌 Example:
```sql
ALTER TABLE EMP_001 ADD EMAILID VARCHAR(50)
```

## **Remove Columns**
### 🧾 Syntax:
```sql
ALTER TABLE <TABLE NAME> DROP COLUMN <COL NAME>
```

### 📌 Example:
```sql
ALTER TABLE EMP_001 DROP COLUMN CONTACT_01
```

## Modify Data Type of Existing Column**
### 🧾 Syntax:
```sql
ALTER TABLE <TABLE NAME> ALTER COLUMN <COL NAME> <NEW DATA TYPE>
```

### 📌 Example:
```sql
ALTER TABLE EMP_001 ALTER COLUMN EMAILID VARCHAR(50)
```

## **Rename Column Name**
### 🧾 Syntax:
```sql
SP_RENMAE '<TABLE NAME>.<OLD COL NAME>', '<NEW COL NAME>'
```

### 📌 Example:
```sql
SP_RENAME 'EMP_001.EMAILID', 'EMAIL'
```

Here's a detailed explanation of the **`TRUNCATE`** statement in SQL:

---

## **TRUNCATE**
- The `TRUNCATE` statement is used to **quickly delete all rows** from a table **without logging each row deletion**.
- It is faster and uses fewer system and transaction log resources than `DELETE`.
- 
### 🧾 Syntax:
```sql
TRUNCATE TABLE table_name;
```

### 🆚 `TRUNCATE` vs `DELETE` vs `DROP`

| Feature          | `TRUNCATE`                                                                      | `DELETE`                                       | `DROP`                             |
| ---------------- | ------------------------------------------------------------------------------- | ---------------------------------------------- | ---------------------------------- |
| Action           | Removes **all rows**                                                            | Removes **selected rows** (or all if no WHERE) | Deletes **entire table structure** |
| `WHERE` clause   | ❌ Not allowed                                                                   | ✅ Allowed                                      | ❌ Not applicable                   |
| Speed            | ✅ Very fast                                                                     | ❌ Slower (row-by-row logging)                  | ✅ Very fast                        |
| Rollback         | ❌ Usually **cannot be rolled back** (unless inside a transaction in some DBMSs) | ✅ Can be rolled back                           | ❌ Cannot be rolled back            |
| Resets identity? | ✅ Yes (in most DBMSs like SQL Server)                                           | ❌ No                                           | ❌ N/A                              |
| Affects schema?  | ❌ No                                                                            | ❌ No                                           | ✅ Yes (removes the table)          |
| Triggers fired?  | ❌ No                                                                            | ✅ Yes                                          | ❌ N/A                              |

### 📌 Example
```sql
-- Before
SELECT COUNT(*) FROM Employees;  -- Output: 1000

-- Truncate the table
TRUNCATE TABLE Employees;

-- After
SELECT COUNT(*) FROM Employees;  -- Output: 0
```

* You **cannot use `TRUNCATE`** on a table that is **referenced by a foreign key constraint**.
* You **cannot truncate** a **specific set of rows** — it's all or nothing.
* In SQL Server: `TRUNCATE` resets `IDENTITY` columns to the seed value.

---

# **DML Commands (Data Manipulation language)**
- Used to manipulate data in tables.
- **INSERT** : Inserting new records
- **UPDATE** : Modifying existing records
- **DELETE** : Delete specific rows from a table (with WHERE clause)

## **INSERT**
- Used to insert new rows in a table
- The order of inserting data must be the same as order of the columns present in a table

### **Method 1 : Supply all the values**
#### 🧾 Syntax:
```sql
INSERT INTO <TABLE>
VALUES ( VALUE1, VALUE2,...)
-- In case I only have a few values then I will mention other values as 'NUll'
```

#### 📌 Example:
```sql
INSERT INTO EMP_001
VALUES ('A1101','ABCD',1000,'01-JAN-2024','HR','A@GMAIL.COM',98121*****)

INSERT INTO EMP_001
VALUES ('A1101','ABCD',1000,'NUll','NUll','NUll','NUll')
```

### **Method 2 : Supply columns for which we are inserting the values**
- Rest of the values will be 'NULL' by default
#### 🧾 Syntax:
```sql
INSERT INTO <TABLE>(<COL 1>, <COL 2>, ... ,<COL n>)
VALUES ( VALUE1, VALUE2,...,VALUEN),
```

#### 📌 Example:
```sql
INSERT INTO EMP_001(EMPID, ENAME)
VALUES ('A1104','PQRS')
```

### **Method 3 : Enter Multiple Records**
#### 🧾 Syntax:
```sql
INSERT INTO <TABLE>(<COL 1>, <COL 2>, ... ,<COL n>)
VALUES ( VALUE1, VALUE2,...,VALUEN),
VALUES ( VALUE1, VALUE2,...,VALUEN),
...
VALUES ( VALUE1, VALUE2,...,VALUEN)
```

#### 📌 Example:
```sql
INSERT INTO EMP_001(EMPID, ENAME)
VALUES ('A1104','PQRS')
VALUES ('A1105','QWER')
VALUES ('A1106','A')
```
## **DELETE**
- Delete all the records, or specified records
### 🧾 Syntax:
```sql
-- all records
DELETE FROM <TABLE>

-- delete specified records
DELETE FROM <TABLE> WHERE <CONDITION>
```

### 📌 Example:
```sql
-- all records
DELETE FROM EMP_001

-- delete specified records
DELETE FROM EMP_001 WHERE EMPID = 'A1106'
```

## **UPDATE**
- Update existing records
### 🧾 Syntax:
```sql
-- all records
UPDATE <TABLE> SET <COL> = <VALUE>

-- UPDATE specified records
UPDATE <TABLE> SET <COL> = <VALUE>
WHERE <CONDITION>
```

### 📌 Example:
```sql
-- all records
UPDATE EMP_001 SET SAL = 25000

-- UPDATE specified records
UPDATE EMP_001 SET SAL = 25000
WHERE EMPID = 'B1101'
```

---

# **CONSTRAINTS**












