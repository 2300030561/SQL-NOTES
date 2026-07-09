# MySQL Installation Guide

## 1. What is MySQL?

MySQL is an open-source Relational Database Management System (RDBMS).

It is used to store, manage, and retrieve data using SQL commands.

Examples of applications using MySQL:
- Banking systems
- E-commerce websites
- Social media applications
- Web applications


---

# 2. MySQL Components

## MySQL Server

- Main database engine
- Stores and manages databases
- Executes SQL queries


## MySQL Client

- Interface used to communicate with MySQL Server
- Example:
  - MySQL Command Line Client
  - MySQL Workbench


## MySQL Workbench

- GUI tool for managing MySQL databases
- Used for:
  - Writing SQL queries
  - Creating databases
  - Designing schemas
  - Viewing tables


---

# 3. System Requirements

Minimum requirements:

- Operating System:
  - Windows
  - Linux
  - macOS

- RAM:
  - Minimum 2GB

- Storage:
  - Around 500MB - 1GB


---

# 4. Installing MySQL on Windows

## Step 1: Download MySQL Installer

Download MySQL Installer from the official MySQL website.

Choose:

MySQL Installer Community Edition


---

## Step 2: Choose Setup Type

Available options:

### Developer Default

Installs:
- MySQL Server
- MySQL Workbench
- MySQL Shell
- Development tools


### Server Only

Installs only MySQL Server


### Custom

Allows selecting required components


Recommended:

Developer Default


---

# 5. MySQL Server Configuration

During installation:

## Authentication Method

Choose:

Strong Password Encryption


## Create Root User

Root user is the administrator account.

Example:

Username:saketh

Password:12345432



Remember this password because it is required to connect to MySQL.


---

# 6. Starting MySQL Server

After installation:

MySQL Server runs as a Windows Service.

Check:


Search:


Status should be:

Running


---

# 7. Connecting to MySQL

Open MySQL Command Line Client.

Enter password:

123454321



If login is successful:

MYSQL



appears.


---

# 8. Verify MySQL Installation

Run:

     sql
SELECT VERSION();
example 
8.0.xx  

SHOW DATABASES;
SHOW DATABASES;
 Creating First Database

Create database:

CREATE DATABASE testdb;

Check database:

SHOW DATABASES;

Use database:

USE testdb;

 MySQL Basic Commands
Show Databases
SHOW DATABASES;
Create Database
CREATE DATABASE database_name;
Delete Database
DROP DATABASE database_name;
Select Database
USE database_name;

 MySQL Workbench Connection

Steps:

Open MySQL Workbench
Click New Connection
Enter:
Connection Name
Username: root
Password
Click Test Connection
Connect


 Common Installation Errors
MySQL Service Not Starting

Solution:

Open services.msc
Restart MySQL service
Access Denied Error

Cause:

Wrong username/password

Solution:

Check root password
Port Error

Default MySQL Port:

3306


 Important Points
MySQL Server stores data
MySQL Workbench provides GUI interface
Root user has complete privileges
Default port is 3306
SQL commands are used to interact with databases
Practice

Tasks:

Install MySQL
Open MySQL Workbench
Create database named company
Create one table
Insert sample data
Retrieve data using SELECT query