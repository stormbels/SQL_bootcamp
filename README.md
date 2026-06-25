SQL Bootcamp

This repository contains my solutions for the SQL Bootcamp tasks.

I use it as a practice project to get more confident with PostgreSQL and relational databases: from simple SELECT queries to joins, indexes, transactions, triggers, and database functions.

The exercises are based on a small pizza ordering database with people, pizzerias, menus, visits, and orders.

⸻

Stack

* PostgreSQL
* DataGrip
* Docker / OrbStack
* SQL
* PL/pgSQL

⸻

About the database

The project uses a small relational model:

* person — people who visit pizzerias and make orders
* pizzeria — restaurants with ratings
* menu — pizzas, prices, and related pizzerias
* person_visits — information about visits
* person_order — information about orders

One important detail: visits and orders are separate entities.
A person can visit one pizzeria and order from another one, so not every task can be solved by simply matching visits and orders directly.

⸻

Structure

The repository is split by days from day00 to day09.

Each day contains:

* materials/ — task materials and database model when needed
* src/ — exercise solutions
* src/exXX/ — a separate folder for each exercise

Example file path:

day00/src/ex00/day00_ex00.sql

⸻

Topics covered

Day 00 — Basic SQL

First queries over the relational model:

* SELECT
* WHERE
* ORDER BY
* DISTINCT
* calculated columns
* CASE
* simple subqueries

Day 01 — Sets and joins

Working with data as sets:

* UNION
* UNION ALL
* INTERSECT
* EXCEPT
* duplicates
* Cartesian product
* basic joins
* IN and EXISTS

Day 02 — More joins

More practice with table relationships:

* LEFT JOIN
* RIGHT JOIN
* FULL JOIN
* missing data
* generate_series
* CTE
* self-joins

Day 03 — Changing data

Working with DML:

* INSERT
* UPDATE
* DELETE
* INSERT INTO ... SELECT
* dynamic ids
* data consistency after changes

Day 04 — Views

Reusable database objects:

* views
* materialized views
* generated date views
* refreshing materialized views
* dropping created objects

Day 05 — Indexes

Query performance basics:

* B-tree indexes
* foreign key indexes
* functional indexes
* multi-column indexes
* unique indexes
* partial indexes
* EXPLAIN ANALYZE

Day 06 — Extending the model

Adding a discount feature:

* new table design
* primary keys
* foreign keys
* constraints
* default values
* comments
* sequences

Day 07 — Aggregations

Getting statistics from data:

* COUNT
* AVG
* MIN
* MAX
* GROUP BY
* HAVING
* rounding and type conversion

Day 08 — Transactions

Working with concurrent sessions:

* transactions
* isolation levels
* READ COMMITTED
* REPEATABLE READ
* SERIALIZABLE
* lost update
* non-repeatable read
* phantom read
* deadlock

Day 09 — Functions and triggers

Database-side logic:

* audit tables
* trigger functions
* insert/update/delete triggers
* generic audit trigger
* SQL functions
* PL/pgSQL functions
* parameterized functions

⸻

Running locally

I run PostgreSQL in Docker / OrbStack.

Connection example:

Host: localhost
Port: 5432
Database: postgres
User: postgres
Password: postgres

Before running the tasks, apply the database model:

day00/materials/model.sql

Then run the exercise files from the corresponding src directory.

⸻

Example query

SELECT
    name,
    age
FROM person
WHERE address = 'Kazan'
ORDER BY name;

⸻

Notes

I keep the solutions split by days and exercises because it is easier to check the progress and return to a specific SQL topic later.

The main purpose of this repository is practice.
I wanted to go through SQL step by step and understand not only how to write queries, but also how PostgreSQL behaves with indexes, transactions, and database-level logic.
