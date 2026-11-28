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

## Tasks 6-7

| Task | Description | SQL Concept |
|------|-------------|-------------|
| 6 | Courses above average enrollment | AVG, HAVING, Subquery |
| 7 | Course enrollment count | LEFT JOIN, COUNT, GROUP BY |

## Task 8 - Integration Scenarios

Database: academy.db

| File | Description |
|------|-------------|
| 8 | Courses and instructors |
| 9 | Instructors and courses |
| 10 | Students and registered courses |
| 11 | Course registration count |
| 12 | Students with registrations |
| 13 | Courses above average assignments |
| 14 | Courses and assignments |
| 15 | Instructors with active courses |

## Final Local Validation

### library.db
- 28 courses.
- 320 enrollments.
- 121 enrolled students.
- Average enrollment: 11.42857.
- 15 courses above average enrollment.
- 2 courses without enrollments.

### academy.db
- 40 courses.
- 420 registrations returned by the join.
- 138 registered students.
- 161 assignments.
- Average assignments per course: 4.025.
- 17 courses above average assignments.
- 25 instructors with active courses.

## Integration Execution

sqlite3 academy.db < file.sql

## Final Reflection

This project demonstrates how relational databases
connect information across multiple tables using
primary keys, foreign keys and junction tables.

JOINs, subqueries, aggregation and correlated
subqueries allow us to retrieve meaningful data
while preserving optional relationships and
producing deterministic results.
