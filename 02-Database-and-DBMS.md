# Database and DBMS

## 1. What is a Database?

A **Database** is an organized collection of data that can be stored, managed, and accessed easily.

A database stores information in a structured format so that users and applications can retrieve data quickly.

### Real-world Examples:

* Student records in a college
* Customer details in a bank
* Product information in an e-commerce website
* Employee records in a company

Example:

Student Database:

| Student_ID | Name | Age | Course |
| ---------- | ---- | --- | ------ |
| 101        | Ravi | 20  | CSE    |
| 102        | Arun | 21  | IT     |

---

# 2. What is DBMS?

**DBMS (Database Management System)** is software that helps users create, store, manage, update, and retrieve data from databases.

It acts as a bridge between the user/application and the database.

### Examples of DBMS:

* MySQL
* Oracle Database
* Microsoft SQL Server
* PostgreSQL
* MongoDB

---

# 3. Why Do We Need DBMS?

Without DBMS:

* Data redundancy increases
* Data security is low
* Data management becomes difficult
* Searching data is slow

With DBMS:

* Data can be stored efficiently
* Security can be maintained
* Multiple users can access data
* Data consistency improves

---

# 4. Components of DBMS

## 1. Hardware

Physical devices used to store and process data.

Examples:

* Servers
* Storage devices
* Computers

## 2. Software

Programs that manage the database.

Examples:

* MySQL
* Oracle

## 3. Data

Actual information stored inside the database.

Example:

* Student details
* Employee records

## 4. Users

People who interact with the database.

Types:

* Database Administrator (DBA)
* Developers
* End Users

## 5. Procedures

Rules and instructions used to manage the database.

---

# 5. Types of Databases

## 1. Relational Database (RDBMS)

Data is stored in tables using rows and columns.

Examples:

* MySQL
* Oracle
* PostgreSQL

Example:

Employee Table:

| ID | Name | Salary |
| -- | ---- | ------ |
| 1  | John | 50000  |

## 2. NoSQL Database

Stores data in flexible formats like documents, key-value pairs, graphs.

Examples:

* MongoDB
* Cassandra

---

# 6. DBMS vs RDBMS

| DBMS                            | RDBMS                           |
| ------------------------------- | ------------------------------- |
| Stores data as files            | Stores data in tables           |
| Less security                   | Higher security                 |
| No relationship between data    | Supports relationships          |
| Suitable for small applications | Suitable for large applications |

---

# 7. Advantages of DBMS

* Reduces data redundancy
* Improves data security
* Provides backup and recovery
* Supports multiple users
* Maintains data consistency
* Faster data access

---

# 8. Disadvantages of DBMS

* Costly software and hardware
* Requires skilled administrators
* Complex to maintain
* Requires more resources

---

# 9. Database Users

## Database Administrator (DBA)

Responsible for:

* Database security
* Backup and recovery
* User permissions
* Performance optimization

## Developers

Responsible for:

* Writing SQL queries
* Creating applications
* Managing database operations

## End Users

Users who access the application and data.

---

# 10. DBMS Architecture

## 1-Tier Architecture

User directly interacts with the database.

Example:

* Local database applications

## 2-Tier Architecture

Client communicates directly with the database server.

Example:

Application → Database

## 3-Tier Architecture

Most commonly used architecture.

Structure:

User
↓
Application Server
↓
Database Server

Example:

Browser → Backend API → Database

---

# Key Points to Remember

* Database = Collection of organized data
* DBMS = Software used to manage databases
* RDBMS stores data in tables
* SQL is used to communicate with relational databases
* MySQL is an example of RDBMS
* DBA manages database security and performance
