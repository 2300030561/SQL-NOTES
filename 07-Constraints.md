# Constraints in MySQL

## What are Constraints?

Constraints are rules applied to table columns to ensure the accuracy, validity, and integrity of data.

They help prevent invalid data from being inserted into a table.

---

# Types of Constraints

1. NOT NULL
2. UNIQUE
3. PRIMARY KEY
4. FOREIGN KEY
5. CHECK
6. DEFAULT

---

# 1. NOT NULL Constraint

## Definition

The NOT NULL constraint ensures that a column cannot contain NULL values.

## Syntax

```sql
CREATE TABLE students (
    id INT,
    name VARCHAR(50) NOT NULL
);
```

---

# 2. UNIQUE Constraint

## Definition

The UNIQUE constraint ensures that all values in a column are different.

## Syntax

```sql
CREATE TABLE students (
    email VARCHAR(100) UNIQUE
);
```

---

# 3. PRIMARY KEY

## Definition

A PRIMARY KEY uniquely identifies each record in a table.

Rules:
- Cannot contain NULL values.
- Must be unique.
- Only one PRIMARY KEY is allowed per table.

## Syntax

```sql
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(50)
);
```

---

# 4. FOREIGN KEY

## Definition

A FOREIGN KEY creates a relationship between two tables.

## Example

```sql
CREATE TABLE departments (
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(50)
);

CREATE TABLE employees (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    dept_id INT,
    FOREIGN KEY (dept_id) REFERENCES departments(dept_id)
);
```

---

# 5. CHECK Constraint

## Definition

The CHECK constraint ensures that values satisfy a specific condition.

## Syntax

```sql
CREATE TABLE students (
    id INT,
    age INT CHECK (age >= 18)
);
```

---

# 6. DEFAULT Constraint

## Definition

The DEFAULT constraint assigns a default value if no value is provided.

## Syntax

```sql
CREATE TABLE employees (
    id INT,
    city VARCHAR(50) DEFAULT 'Hyderabad'
);
```

---

# Example Table Using Multiple Constraints

```sql
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    age INT CHECK(age >= 18),
    city VARCHAR(50) DEFAULT 'Hyderabad'
);
```

---

# Difference Between PRIMARY KEY and UNIQUE

| PRIMARY KEY | UNIQUE |
|-------------|--------|
| Only one per table | Multiple UNIQUE constraints allowed |
| Cannot contain NULL | Can contain NULL (MySQL behavior depends on version/settings) |
| Must be unique | Must be unique |

---

# Advantages of Constraints

- Improves data integrity
- Prevents invalid data
- Maintains consistency
- Creates relationships between tables
- Reduces duplicate records

---

# Interview Questions

### 1. What are Constraints?

Constraints are rules that enforce data integrity in a database table.

### 2. Name the different types of Constraints.

- NOT NULL
- UNIQUE
- PRIMARY KEY
- FOREIGN KEY
- CHECK
- DEFAULT

### 3. Can a table have multiple PRIMARY KEYs?

No. A table can have only one PRIMARY KEY.

### 4. What is the purpose of a FOREIGN KEY?

It creates a relationship between two tables and maintains referential integrity.

### 5. What is the difference between PRIMARY KEY and UNIQUE?

PRIMARY KEY uniquely identifies each row and cannot contain NULL values, whereas UNIQUE also enforces uniqueness but can allow NULL values depending on the database system.

### 6. Why is NOT NULL used?

To ensure that a column always contains a value and never stores NULL.

### 7. What is the purpose of the DEFAULT constraint?

It automatically assigns a predefined value when no value is provided during insertion.