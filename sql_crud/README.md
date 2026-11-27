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

## Task 7 - Ordering and Limiting Results

| File | Description |
| --- | --- |
| 7-order_by_price_asc.sql | Sorts books by ascending price. |
| 7-order_by_year_desc.sql | Sorts books by descending publication year. |
| 7-limit_results.sql | Returns the three cheapest books. |
| 7-order_and_limit.sql | Returns the five books with highest stock. |

### Concepts Learned

- ORDER BY controls the order of query results.
- ASC sorts values in ascending order.
- DESC sorts values in descending order.
- LIMIT restricts the number of returned rows.
- Sorting occurs before limiting the result set.

Local validation: All four queries passed.

## Task 8 - Aggregate Functions

| File | Description |
| --- | --- |
| 8-count_books.sql | Counts all books. |
| 8-average_price.sql | Calculates the average price. |
| 8-max_stock.sql | Finds the maximum stock value. |
| 8-total_stock.sql | Calculates the total available stock. |
| 8-min_price.sql | Finds the minimum price. |

### Concepts Learned

- COUNT counts records.
- AVG calculates the arithmetic mean.
- MAX returns the largest value.
- SUM adds numerical values.
- MIN returns the smallest value.
- Aggregate functions summarize multiple rows into one value
  when used without grouping.

Local validation: All five queries passed.
