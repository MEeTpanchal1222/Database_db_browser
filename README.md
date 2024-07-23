


# Employee Management SQL Operations

This repository contains SQL scripts for managing an `employees` table. The table includes columns for name, role, salary, age, and phone number. Below are the details of the table structure and various SQL operations performed.

## Table Structure

```sql
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    role VARCHAR(255),
    salary INT,
    age INT,
    phone VARCHAR(255)
);
```

## Data Insertion

Inserting data into the `employees` table:

```sql
INSERT INTO employees (name, role, salary, age, phone) VALUES ("John", "ceo", 120000, 35, 9812345678);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Jane", "hr", 85000, 30, 8823456789);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Alice", "manager", 78000, 28, 8734567890);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Bob", "emp", 90000, 25, 8645678901);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Charlie", "emp", 98000, 27, 8556789012);
INSERT INTO employees (name, role, salary, age, phone) VALUES ("Dave", "emp", 62000, 22, 8467890123);
```

## Data Retrieval

Selecting all data from the `employees` table:

```sql
SELECT * FROM employees;
```

Selecting specific columns:

```sql
SELECT name FROM employees;
SELECT salary FROM employees;
```

Filtering data based on conditions:

```sql
SELECT * FROM employees WHERE role = "manager";
SELECT * FROM employees WHERE name LIKE 'A%';
SELECT * FROM employees WHERE (age > 25 AND salary > 85000);
```

## Data Update

Updating data in the `employees` table:

```sql
UPDATE employees SET salary = 55000 WHERE id = 2;
UPDATE employees SET phone = 8678901234 WHERE id = 4;
```

## Data Deletion

Deleting data from the `employees` table:

```sql
DELETE FROM employees WHERE id = 6;
DELETE FROM employees WHERE age > 30;
```
