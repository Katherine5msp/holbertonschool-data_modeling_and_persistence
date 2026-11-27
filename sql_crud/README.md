# SQL - CRUD Operations

This project introduces relational databases and SQL
using SQLite. It covers table creation, CRUD operations,
filtering, ordering, aggregation, and grouping.

## Environment

- Ubuntu 20.04
- SQLite 3.x

## Tasks

### Task 0 - Understanding and Creating a Table

File: 0-create_table.sql

Creates a books table with seven columns, appropriate
data types, a primary key, and NOT NULL constraints.

Local validation: Successful.

### Task 1 - Inserting Data into a Table

File: 1-insert_data.sql

Uses INSERT INTO to populate the books table with five
predefined records, explicitly mapping values to columns.

Local validation: Successful.
All five records and their values were verified.

### Task 2 - Retrieving All Data from a Table

File: 2-select_all.sql

Uses SELECT * to retrieve all rows and columns
from the books table without modifying the data.

Local validation: Five records returned successfully.

### Task 3 - Selecting Specific Columns

File: 3-select_columns.sql

Uses SELECT to retrieve specific columns (title and price)
from the books table without filtering or modifying data.

Local validation: Successful.
Five rows and two columns returned correctly.


## Task 4 - Filtering Rows

| File | Description |
| --- | --- |
| 4-filter_by_genre.sql | Filters books by genre. |
| 4-filter_by_price.sql | Filters books by price. |
| 4-filter_with_and.sql | Combines conditions using AND. |
| 4-filter_with_or.sql | Combines conditions using OR. |

### Concepts Learned

- WHERE filters rows based on conditions.
- Comparison operators filter numerical values.
- AND requires both conditions to be true.
- OR requires at least one condition to be true.
- SELECT returns only the requested columns.

All four queries were successfully tested using a temporary
local SQLite database.


## Task 5 - Updating Rows

| File | Description |
| --- | --- |
| 5-update_by_id.sql | Updates a price using the primary key. |
| 5-update_by_condition.sql | Increases stock based on publication year. |
| 5-update_with_and.sql | Applies a discount using compound conditions. |

### Concepts Learned

- UPDATE modifies existing records.
- SET assigns or calculates new values.
- WHERE restricts which rows are modified.
- Primary keys uniquely identify records.
- Independent database copies prevent test interference.

Local validation: All three queries passed.

## Task 6 - Deleting Rows

| File | Description |
| --- | --- |
| 6-delete_by_id.sql | Deletes a record using its primary key. |
| 6-delete_by_condition.sql | Deletes books with zero stock. |
| 6-delete_with_and.sql | Deletes records matching compound conditions. |

### Concepts Learned

- DELETE removes entire records.
- WHERE restricts which records are deleted.
- AND requires both conditions to be true.
- SELECT can preview records before deletion.
- Independent database copies protect original data.

Local validation: All three queries passed using a
temporary database with synthetic test records.
