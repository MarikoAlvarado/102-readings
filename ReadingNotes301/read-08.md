# [SQLBolt Lessons 1-4 & 13-18](https://sqlbolt.com/)

## SQL

- SQL = Structure Query Language

- Designed for technical & non-technical: query, manipulate, data transform from relational database.

- Safe and scalable storage

**Relational Database**

- represents a collection of two-dimensional tables

- named columns = attributes/properties of table

- rows = data

**SELECT** 

- Often referred to as *queries*, a statement that declares the **data being looked for**
**BASIC EXAMPLE

### Queries with constraints

- complex clauses can be constructed by joining multiple ``AND`` ``OR`` keywords and with use of **operators**.

- using ``WHERE``, SQL supports the use of text-data specific operators

### Filtering and sorting

- ``DISTINCT`` blindly discards rows with duplicate column values

- ``GROUP BY`` lets use discard based on specific columns

- ``ORDER BY`` allows organization by **ascending** or **descending** order. Often used with:

  - ``LIMIT`` to reduced number of rows to return

  - ``OFFSET`` to specify where to begin counting of number of rows from 

### Inserting, Updating, Deleting, Creating, Altering & Dropping

- **Database Schema** describes structure of table and datatypes each table can have.

- ``INSERT`` declares which table to write into, columns of data to fill and one + rows of data to insert

- ``UPDATE`` similar to INSERT but the **data**  being updated *must* match data type of columns in **table schema**

- ``DELETE`` describes table to act on and which rows to delete using ``WHERE`` clause.

- ``CREATING`` can be made with different table types and each column can have table **constraints**

- ``ALTER TABLE`` to **add**, **remove**, or **modify** columns and constraints

- ``DROP TABLE`` **different from DELETE** because it also *removes* table schema from database *entirely*
