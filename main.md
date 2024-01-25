## Updating a Value:

```sql
Copy code
UPDATE employees SET salary = 50000 WHERE employee_id = 123;
```
## Adding a New Column:

```sql
Copy code
ALTER TABLE employees ADD email VARCHAR(255);
```

## Deleting a Row:

```sql
Copy code
DELETE FROM employees WHERE employee_id = 456;
```

## Selecting Data with Conditions:

```sql
Copy code
SELECT * FROM employees WHERE salary > 30000;
```

## Creating a New Table:

```sql
Copy code
CREATE TABLE departments (department_id INT PRIMARY KEY, department_name VARCHAR(100));
```
## Joining Tables:

```sql
Copy code
SELECT employees.name, departments.department_name FROM employees INNER JOIN departments ON employees.department_id = departments.department_id;
```

## Grouping and Aggregating Data:

```sql
Copy code
SELECT department_id, AVG(salary) AS average_salary FROM employees GROUP BY department_id;
```

## Using Subqueries:

```sql
Copy code
SELECT name, salary FROM employees WHERE salary > (SELECT AVG(salary) FROM employees);
```

## Updating Data Based on Conditions:

```sql
Copy code
UPDATE employees SET salary = salary * 1.10 WHERE salary < 30000;
```

## Using LIKE for Pattern Matching:

```sql
Copy code
SELECT * FROM employees WHERE name LIKE 'J%';
```

## Limiting Query Results:

```sql
Copy code
SELECT * FROM employees ORDER BY employee_id LIMIT 5;
```

## Creating Indexes:

```sql
Copy code
CREATE INDEX idx_salary ON employees (salary);
```

These examples cover various fundamental SQL operations, from basic data manipulation to more complex queries and database management techniques.
