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

\
\










