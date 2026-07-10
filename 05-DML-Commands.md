# DML (Data Manipulation Language)

## What is DML?

DML stands for **Data Manipulation Language**.

It is used to **insert, update, and delete data** from a table.

**DML Commands:**
- INSERT
- UPDATE
- DELETE

---

# 1. INSERT Command

## Definition

The INSERT command is used to add new records into a table.

## Syntax

```sql
INSERT INTO table_name (column1, column2, column3)
VALUES (value1, value2, value3);
```

## Example

```sql
CREATE TABLE students (
    id INT,
    name VARCHAR(50),
    age INT
);

INSERT INTO students (id, name, age)
VALUES (1, 'Saketh', 21);
```

## Output

| id | name   | age |
|----|--------|-----|
| 1  | Saketh | 21  |

---

# 2. UPDATE Command

## Definition

The UPDATE command is used to modify existing records in a table.

## Syntax

```sql
UPDATE table_name
SET column_name = value
WHERE condition;
```

## Example

```sql
UPDATE students
SET age = 22
WHERE id = 1;
```

## Output

| id | name   | age |
|----|--------|-----|
| 1  | Saketh | 22  |

---

# 3. DELETE Command

## Definition

The DELETE command is used to remove records from a table.

## Syntax

```sql
DELETE FROM table_name
WHERE condition;
```

## Example

```sql
DELETE FROM students
WHERE id = 1;
```

---

# Difference Between INSERT, UPDATE and DELETE

| Command | Purpose |
|----------|---------|
| INSERT | Adds new records |
| UPDATE | Modifies existing records |
| DELETE | Removes existing records |

---

# Important Points

- INSERT adds new rows.
- UPDATE changes existing data.
- DELETE removes selected rows.
- Always use the **WHERE** clause with UPDATE and DELETE to avoid affecting all records.

---

# Interview Questions

### 1. What is DML?

DML (Data Manipulation Language) is used to insert, update, and delete data from database tables.

### 2. Which commands belong to DML?

- INSERT
- UPDATE
- DELETE

### 3. What happens if UPDATE is executed without a WHERE clause?

It updates **all rows** in the table.

### 4. What happens if DELETE is executed without a WHERE clause?

It deletes **all rows** from the table.

### 5. Which command is used to add new records?

**INSERT**