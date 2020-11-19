# [Database Normalization](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

A process for organizing a database into tables and columns. Each table should only feature things sharing a *specific topic*. If each table has it's own purpose, there is a lower chance of duplicating the data stored within your database and can keep you from having to deal with db modifications and the possible side affects. 

Reasons to **normalize a database**:
- minimize duplicate data
- minimize/avoid data modification issues
- simplify queries

*remember*..It's best for tables to have a single purpose.

**Insert Anomaly**- in order to create a record of something you need a **primary key**

**Update Anomaly**- If all rows are *not* updated, **inconsistencies** will appear.

#### Definition of Database Normalization

**First Formal Form**

- Data is stored in relational table, each column holding *atomic* values. No repeating groups of columns

**Second Normal Form**

- Table is in first normal form and the columns depend on table's **primary key**

**Third Normal Form**

- Table is at second normal forms, all columns are **not** dependent on primary key.

