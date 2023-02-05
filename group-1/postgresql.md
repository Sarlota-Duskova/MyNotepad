# PostgreSQL

The capitalized words are keywords telling PostgreSQL what to do. All commands need a semi-colon at the end.

`\l` - list of database

`\c database_name` - enter into a database

`\d` - when I am in that database show tables

`\d first_table` - view more details about a table

`VARCHAR(30)` - a short string of characters

The `SERIAL` type will make your column an `INT` with a `NOT NULL` constraint, and automatically increment the integer when a new row is added.&#x20;

Enter into a database:

```sql
psql --username=freecodecamp --dbname=postgres
```

Create Database:

```sql
CREATE DATABASE first_database ;
```

Create a table inside a database:

```sql
CREATE TABLE table_name();
```

Add column into a table:

```sql
ALTER TABLE table_name ADD COLUMN column_name DATATYPE;
```

Delete column in a table:

```sql
ALTER TABLE table_name DROP COLUMN column_name;
```

Rename column name:

```sql
ALTER TABLE table_name RENAME COLUMN column_name TO new_name;
```

Add rows into a table:

```sql
INSERT INTO table_name(column_1, column_2) VALUES(value1, value2);
```

View the data in a table:

```sql
SELECT columns FROM table_name;
```

Delete a row:

```sql
DELETE FROM table_name WHERE condition;
```

condition could be `username='Luigi'`\
\
Delete table:

```sql
DROP TABLE table_name;
```

Empty the rows in the tables of your database with:

```sql
 TRUNCATE TABLE table_name1, table_name2;
```

Delete database:

```sql
DROP DATABASE table_name;
```

Update:

```sql
UPDATE table_name SET column_name=new_value WHERE condition;
```

Put the table into order:

```sql
SELECT columns FROM table_name ORDER BY column_name;
It's a column that uniquely identifies each row in the table.
```

Set Primary key. It's a column that uniquely identifies each row in the table.

```sql
ALTER TABLE table_name ADD PRIMARY KEY(column_name);
```

```sql
ALTER TABLE table_name DROP CONSTRAINT constraint_name;
```

**Foreign key** can relate rows from this table to rows from your another table.&#x20;

```sql
ALTER TABLE table_name ADD COLUMN column_name DATATYPE REFERENCES referenced_table_name(referenced_column_name);
```

```sql
ALTER TABLE table_name ADD FOREIGN KEY(column_name) REFERENCES table_name(column_name);
```

These tables have a "one-to-one" relationship. **One** row in the `characters` table will be related to exactly **one** row in `more_info` and vice versa. Enforce that by adding the `UNIQUE` constraint to your foreign key. Here's an example:

```sql
ALTER TABLE table_name ADD UNIQUE(column_name);
```

The column should also be `NOT NULL` since you don't want to have a row that is for nobody. Here's an example:

```sql
ALTER TABLE table_name ALTER COLUMN column_name SET NOT NULL;
```

This will be a "one-to-many" relationship because **one** character will have **many** sounds, but no sound will have more than one character.&#x20;

```sql
ALTER TABLE table_name ADD COLUMN column_name DATATYPE CONSTRAINT REFERENCES referenced_table_name(referenced_column_name);
```

You can create a primary key from two columns, known as a **composite** primary key.&#x20;

```sql
ALTER TABLE table_name ADD PRIMARY KEY(column1, column2);
```

`LIKE` - find a pattern in text&#x20;

`ILIKE` - will ignore the case of the letters

`NOT LIKE` - to find things that don't match a pattern

`IS NULL` - view all data that is null

`IS NOT NULL` -view all data that is not null

An underscore (`_`) in a pattern will return rows that have any character in that spot.

`%` - anything can be there.

```sql
SELECT columns FROM table_name WHERE column ILIKE '%A%';
```

`ORDER BY <column_name>` at the end of a query

it will be in ascending (`ASC`) order by default. Add `DESC` (descending) at the end of the last query to put the highest ones at the top.

`LIMIT <number>` at the end of the query to only get the amount you want.

`SELECT MIN(<column>) FROM <table>`. It will find the lowest value in the column.&#x20;

`MAX`

`SUM`

`AVG` will give you the average of all the values in a column.&#x20;

Round decimals up or down to the nearest whole number with `CEIL` and `FLOOR`

Round a number to the nearest whole number with `ROUND`

`ROUND(<number_to_round>, <decimals_places>)`

`COUNT(<column>)` - It will tell how many entries are in a table for the column.

`DISTINCT` is a function that will show you only unique values.

```sql
SELECT DISTINCT(column) FROM table;
```

```sql
SELECT <column> FROM <table> GROUP BY <column>
```

Another option with `GROUP BY` is `HAVING`.

Rename a column with `AS`

```sql
SELECT <column> AS <new_column_name>
```

`JOIN` the two tables into one.&#x20;

The `FULL JOIN` you used will include **all** rows from both tables, whether or not they have a row using that foreign key in the other.

```sql
SELECT * FROM <table_1> FULL JOIN <table_2> ON <table_1>.<foreign_key_column> = <table_2>.<foreign_key_column>;
```

`LEFT JOIN` to join the same two tables in the same way.

`RIGHT JOIN`

Join the two tables with an `INNER JOIN` - it only returned rows if they have a value in the foreign key column of the opposite table.&#x20;

`<table>.<column>` - specify what table you want the column from

Rename tables, or give them aliases, as well. Here's an example: `SELECT * FROM <table> AS <new_name>;`

`USING` to join tables if the foreign key column has the same name in both tables.

```sql
SELECT * FROM <table_1> FULL JOIN <table_2> USING(<column>);
```

Join multiple tables

```sql
SELECT * FROM <table_1> FULL JOIN <table_2> USING(<column>) FULL JOIN <table_3> USING(<column>)
```

Dump of database:

```sql
You can make a dump of it by entering pg_dump -cC --inserts -U freecodecamp worldcup > worldcup.sql
```









