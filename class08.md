# SQL  

When working with multiple tables, the UNION and UNION ALL operator allows you to append the results of one query to another assuming that they have the same column count, order and data type. If you use the UNION without the ALL, duplicate rows between the tables will be removed from the result. 

In the order of operations as defined in Lesson 12: Order of execution, the UNION happens before the ORDER BY and LIMIT. It's not common to use UNIONs, but if you have data in different tables that can't be joined and processed, it can be an alternative to making multiple queries on the database.

Similar to the UNION, the INTERSECT operator will ensure that only rows that are identical in both result sets are returned, and the EXCEPT operator will ensure that only rows in the first result set that aren't in the second are returned. This means that the EXCEPT operator is query order-sensitive, like the LEFT JOIN and RIGHT JOIN.


you can think of a table in SQL as a type of an entity (ie. Dogs), and each row in that table as a specific instance of that type 

## Queries with constraints :

In order to filter certain results from being returned, we need to use a ***WHERE*** clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not. 


When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching. 


## Filtering and sorting Query results 

SQL provides a convenient way to discard rows that have a duplicate column value by using the ***DISTINCT*** keyword.
the #### DISTINCT keyword will blindly remove duplicate rows

When an ***ORDER BY*** clause is specified, each row is sorted alpha-numerically based on the specified column's value. In some databases, you can also specify a collation to better sort data containing international text.

Another clause which is commonly used with the ***ORDER BY*** clause are the **LIMIT** and **OFFSET** clauses, which are a useful optimization to indicate to the database the subset of the results you care about.
The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.

## Inserting rows 

In SQL, the database schema is what describes the structure of each table, and the datatypes that each column of the table can contain. 

When inserting data into a database, we need to use an **INSERT** statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. In general, each row of data you insert should contain values for every corresponding column in the table. You can insert multiple rows at a time by just listing them sequentially.


`INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …; `

## Updating rows 

***UPDATE*** statement. Similar to the INSERT statement, you have to specify exactly which table, columns, and rows to update. In addition, the data you are updating has to match the data type of the columns in the table schema.

The statement works by taking multiple column/value pairs, and applying those changes to each and every row that satisfies the constraint in the WHERE clause.

##  Deleting rows 

 ***DELETE*** statement, which describes the table to act on, and the rows of the table to delete through the WHERE clause. 

`DELETE FROM mytable
WHERE condition;`


## Creating tables 


`CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,

##  Altering tables


SQL provides a way for you to update your corresponding tables and database schemas by using the ***ALTER TABLE*** statement to add, remove, or modify columns and table constraints.






    …
);`
