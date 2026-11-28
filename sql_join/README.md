# SQL - Joins & Relationships

## Description
This project explores relational databases, table
relationships, SQL joins, subqueries and aggregation.

## Environment
- Ubuntu 20.04
- SQLite 3.31.1

## Task 0 - Understanding Table Relationships

### Database Tables
- authors
- books
- students
- courses
- enrollments

### Relationships
- Authors to books: one-to-many.
- Students to enrollments: one-to-many.
- Courses to enrollments: one-to-many.
- Students to courses: many-to-many.

### Key Concepts
- Primary keys uniquely identify records.
- Foreign keys establish relationships between tables.
- Composite keys combine multiple columns.
- Junction tables connect many-to-many relationships.
- Referential integrity maintains valid relationships.

### Execution
sqlite3 library.db < file.sql

