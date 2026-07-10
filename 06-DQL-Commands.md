# DQL (Data Query Language)

## What is DQL?

DQL stands for **Data Query Language**.

It is used to retrieve (fetch) data from one or more tables in a database.

**DQL Command:**
- SELECT

---

# SELECT Command

## Definition

The SELECT command is used to retrieve data from a table.

## Syntax

```sql
SELECT column_name
FROM table_name;
```

## Example

```sql
SELECT * FROM students;
```

## Output

| id | name   | age |
|----|--------|-----|
| 1  | Saketh | 21  |
| 2  | Rahul  | 22  |

---

# Selecting Specific Columns

## Syntax

```sql
SELECT column1, column2
FROM table_name;
```

## Example

```sql
SELECT name, age
FROM students;
```

---

# SELECT DISTINCT

## Definition

DISTINCT is used to display only unique values.

## Syntax

```sql
SELECT DISTINCT column_name
FROM table_name;
```

## Example

```sql
SELECT DISTINCT department
FROM employees;
```

---

# WHERE Clause

## Definition

The WHERE clause is used to filter records based on a condition.

## Syntax

```sql
SELECT *
FROM table_name
WHERE condition;
```

## Example

```sql
SELECT *
FROM students
WHERE age > 20;
```

---

# ORDER BY

## Definition

ORDER BY is used to sort the result in ascending or descending order.

## Syntax

```sql
SELECT *
FROM table_name
ORDER BY column_name ASC;
```

or

```sql
SELECT *
FROM table_name
ORDER BY column_name DESC;
```

## Example

```sql
SELECT *
FROM students
ORDER BY age DESC;
```

---

# LIMIT

## Definition

LIMIT is used to restrict the number of rows returned.

## Syntax

```sql
SELECT *
FROM table_name
LIMIT number;
```

## Example

```sql
SELECT *
FROM students
LIMIT 5;
```

---

# Aliases (AS)

## Definition

Aliases are used to give a temporary name to a column.

## Syntax

```sql
SELECT column_name AS alias_name
FROM table_name;
```

## Example

```sql
SELECT name AS Student_Name
FROM students;
```

---

# Important Points

- SELECT retrieves data from a table.
- WHERE filters records.
- DISTINCT removes duplicate values.
- ORDER BY sorts data.
- LIMIT restricts the number of rows.
- AS creates a temporary column name.

---

# Interview Questions

### 1. What is DQL?

DQL (Data Query Language) is used to retrieve data from a database.

### 2. Which command belongs to DQL?

**SELECT**

### 3. What is the use of DISTINCT?

It removes duplicate values and displays only unique records.

### 4. What is the use of WHERE?

It filters records based on a condition.

### 5. What is the use of ORDER BY?

It sorts data in ascending or descending order.

### 6. What is the use of LIMIT?

It restricts the number of rows returned.

### 7. What is the purpose of the AS keyword?

It gives a temporary alias (name) to a column or table.