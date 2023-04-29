# relational databases and SQL

## summary
**SELECT** is a keyword used in SQL (Structured Query Language) to retrieve data from one or more tables in a database. A SELECT query allows you to specify the columns of data you want to retrieve, as well as the conditions under which you want to retrieve them.

The basic syntax for a SELECT query is:
```
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```
The SELECT statement specifies which columns you want to retrieve from the table. You can select all columns by using *. The FROM clause specifies which table you want to retrieve data from. The WHERE clause is optional, but allows you to filter the data based on a specific condition.

For example, the following query retrieves all columns from the "customers" table where the "country" column is equal to "USA":
```
SELECT *
FROM customers
WHERE country = 'USA';
```
![task1](https://user-images.githubusercontent.com/125543324/235305599-40107976-73aa-40e3-94f3-3518e47de205.png)

### Queries with **constraints** are used to filter the data that is returned by the query.
For example, the following query retrieves all rows from the "employees" table where the "salary" column is greater than $50,000:
```
SELECT *
FROM employees
WHERE salary > 50000;
```
### Other types of constraints include:

**AND** and **OR** operators: These operators are used to combine multiple constraints in a single query. For example, the following query retrieves all rows from the "employees" table where the "salary" column is greater than $50,000 and the "department" column is equal to "Marketing":
```
SELECT *
FROM employees
WHERE salary > 50000 AND department = 'Marketing';
```
### **IN** operator: This operator is used to match a value against a list of possible values.
For example, the following query retrieves all rows from the "employees" table where the "department" column is either "Marketing" or "Sales":
```
SELECT *
FROM employees
WHERE department IN ('Marketing', 'Sales');
```
### **LIKE** operator: This operator is used to match a value against a pattern. 
For example, the following query retrieves all rows from the "employees" table where the "last_name" column starts with "Smi":
```
SELECT *
FROM employees
WHERE last_name LIKE 'Smi%';
```
![task2](https://user-images.githubusercontent.com/125543324/235305971-52f42317-9aad-4d88-9d7d-71999c85b1b9.png)
![task3](https://user-images.githubusercontent.com/125543324/235306045-930c8968-6038-48ea-b9ad-e339138f153a.png)

### **Sorting** is done using the ORDER BY clause, which allows you to specify the order in which the rows should be returned. 
For example, the following query retrieves all rows from the "orders" table and sorts them by the "order_date" column in ascending order:
```
SELECT *
FROM orders
ORDER BY order_date ASC;
```
### You can also sort in descending order by using the **DESC** keyword, like this:
```
SELECT *
FROM orders
ORDER BY order_date DESC;
```
### you can also limit the number of rows returned by a query using the **LIMIT** clause. 
For example, the following query retrieves the first 10 rows from the "customers" table:
```
SELECT *
FROM customers
LIMIT 10;
```
![task4](https://user-images.githubusercontent.com/125543324/235306268-c056d221-f9a8-4f97-88e6-583503eec763.png)

![task5](https://user-images.githubusercontent.com/125543324/235306327-f5729f46-6de2-4e6f-a59d-3030729b6c61.png)

### The basic syntax for an **INSERT** statement is as follows:
```
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

TO inserts a new row into the "customers" table:
```
INSERT INTO customers (first_name, last_name, age)
VALUES ('Rna', 'ahmed', '27');
```
If you want to insert multiple rows at once, you can use a comma-separated list of value sets in the VALUES clause. For example, the following query inserts two new rows into the "customers" table:

```
INSERT INTO customers (first_name, last_name, age)
VALUES ('sally', 'ayman', '33'),
       ('sally', 'ayman', '33');
```

![task13](https://user-images.githubusercontent.com/125543324/235307568-f0ee4f14-82a1-49b0-9a7c-f1eef1dbd05c.png)

### The basic syntax for an **UPDATE** statement is as follows:

```
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

![task14](https://user-images.githubusercontent.com/125543324/235309325-d07b8412-568c-4482-ba6f-447378f0e1e2.png)

### The basic syntax for an **DELETE** statement is as follows:

```
DELETE FROM mytable
WHERE condition;
```

![Task15](https://user-images.githubusercontent.com/125543324/235309472-5f10dd21-4f34-40dd-9302-48802e3021a4.png)

### The basic syntax for a **CREATE TABLE** statement is as follows:

```
CREATE TABLE table_name (
  column1 datatype constraints,
  column2 datatype constraints,
  column3 datatype constraints,
  ...
);
```

![Task16](https://user-images.githubusercontent.com/125543324/235309651-4f4bee43-9440-4cae-857f-15ef591d0f26.png)

### The basic syntax for an **ALTER TABLE** statement is as follows:

```
ALTER TABLE table_name
ADD column_name datatype constraints;

ALTER TABLE table_name
RENAME TO new_table_name;

ALTER TABLE table_name
DROP COLUMN column_name;
```

![task17](https://user-images.githubusercontent.com/125543324/235310000-7cad6e29-ab75-4636-931f-b7d6b7b2bf97.png)

### The basic syntax for an **DROP TABLE** statement is as follows:

```
DROP TABLE table_name;
```

![task18](https://user-images.githubusercontent.com/125543324/235310146-59d7123a-4489-4f4d-a300-e724b179b416.png)
