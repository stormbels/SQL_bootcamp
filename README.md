<img align="right" src="images/pg_elephant_pizza.png" alt="PostgreSQL elephant with pizza" width="380"/>

# SQL Bootcamp 🍕🐘

*(PostgreSQL practice project)*

I never thought pizza orders could teach me so much about databases 😳

This repository contains my solutions for the SQL Bootcamp tasks 🎓

The project starts with a small pizza ordering database and gradually moves
from simple `SELECT` queries to joins, indexes, transactions, triggers, and functions 💆🏽‍♀️

<br clear="right"/>
<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 🎯 What is this project about?

1. People visit pizzerias 👣
2. Pizzerias have menus 🍕
3. People make orders 🧾
4. Orders are linked to menu items, not directly to visits 🔗
5. Later days add discounts, views, indexes, audit tables, triggers, sequences, and functions ⚙️
6. PostgreSQL watches my queries and says: "Are you sure?" 🫣

<img src="images/joins.png" alt="Joins" width="600"/>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

<img src="images/important_detail.png" alt="Important detail" width="600"/><br>
<img src="images/get_pizza.png" alt="Visit and order are separate entities" width="600"/>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 🛠️ Tech Stack

![SQL](https://img.shields.io/badge/-SQL-4479A1?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?logo=postgresql&logoColor=white&style=for-the-badge)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge)
![OrbStack](https://img.shields.io/badge/-OrbStack-8B5CF6?style=for-the-badge)

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 🔍 About the database

The project starts with a small relational model and later extends it with additional database objects:

<img src="images/database.png" alt="Database" width="600"/>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 🧩 Project layout

Solutions are split by days from `day00` to `day09`

Each day contains exercise folders with SQL files inside

Example:

<img src="images/repository.png" alt="Project folder structure" width="600"/>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 📚 Topics covered

<img src="images/first_days.png" alt="SQL Bootcamp first days" width="850"/>

<table>
  <tr>
    <th>Day 00<br>Basic SQL</th>
    <th>Day 01<br>Sets and joins</th>
    <th>Day 02<br>More joins</th>
    <th>Day 03<br>Changing data</th>
    <th>Day 04<br>Views</th>
  </tr>
  <tr>
    <td valign="top">
      First queries over the relational model:
      <br><br>
      <ul>
        <li><code>SELECT</code></li>
        <li><code>WHERE</code></li>
        <li><code>ORDER BY</code></li>
        <li><code>DISTINCT</code></li>
        <li>calculated columns</li>
        <li><code>CASE</code></li>
        <li>simple subqueries</li>
      </ul>
    </td>
    <td valign="top">
      Working with data as sets:
      <br><br>
      <ul>
        <li><code>UNION</code></li>
        <li><code>UNION ALL</code></li>
        <li><code>INTERSECT</code></li>
        <li><code>EXCEPT</code></li>
        <li>duplicates</li>
        <li>Cartesian product</li>
        <li>basic joins</li>
        <li><code>IN</code> and <code>EXISTS</code></li>
      </ul>
    </td>
    <td valign="top">
      More practice with table relationships:
      <br><br>
      <ul>
        <li><code>LEFT JOIN</code></li>
        <li><code>RIGHT JOIN</code></li>
        <li><code>FULL JOIN</code></li>
        <li>missing data</li>
        <li><code>generate_series</code></li>
        <li>CTE</li>
        <li>self-joins</li>
      </ul>
    </td>
    <td valign="top">
      Working with DML:
      <br><br>
      <ul>
        <li><code>INSERT</code></li>
        <li><code>UPDATE</code></li>
        <li><code>DELETE</code></li>
        <li><code>INSERT INTO ... SELECT</code></li>
        <li>dynamic ids</li>
        <li>data consistency after changes</li>
      </ul>
    </td>
    <td valign="top">
      Reusable database objects:
      <br><br>
      <ul>
        <li>views</li>
        <li>materialized views</li>
        <li>generated date views</li>
        <li>refreshing materialized views</li>
        <li>dropping created objects</li>
      </ul>
    </td>
  </tr>
</table>

<img src="images/second_days.png" alt="SQL Bootcamp second days" width="850"/>

<table>
  <tr>
    <th>Day 05<br>Indexes</th>
    <th>Day 06<br>Extending the model</th>
    <th>Day 07<br>Aggregations</th>
    <th>Day 08<br>Transactions</th>
    <th>Day 09<br>Functions and triggers</th>
  </tr>
  <tr>
    <td valign="top">
      Query performance basics:
      <br><br>
      <ul>
        <li>B-tree indexes</li>
        <li>foreign key indexes</li>
        <li>functional indexes</li>
        <li>multi-column indexes</li>
        <li>unique indexes</li>
        <li>partial indexes</li>
        <li><code>EXPLAIN ANALYZE</code></li>
      </ul>
    </td>
    <td valign="top">
      Adding a discount feature:
      <br><br>
      <ul>
        <li>new table design</li>
        <li>primary keys</li>
        <li>foreign keys</li>
        <li>constraints</li>
        <li>default values</li>
        <li>comments</li>
        <li>sequences</li>
      </ul>
    </td>
    <td valign="top">
      Getting statistics from data:
      <br><br>
      <ul>
        <li><code>COUNT</code></li>
        <li><code>AVG</code></li>
        <li><code>MIN</code></li>
        <li><code>MAX</code></li>
        <li><code>GROUP BY</code></li>
        <li><code>HAVING</code></li>
        <li>rounding and type conversion</li>
      </ul>
    </td>
    <td valign="top">
      Working with concurrent sessions:
      <br><br>
      <ul>
        <li>transactions</li>
        <li>isolation levels</li>
        <li><code>READ COMMITTED</code></li>
        <li><code>REPEATABLE READ</code></li>
        <li><code>SERIALIZABLE</code></li>
        <li>lost update</li>
        <li>non-repeatable read</li>
        <li>phantom read</li>
        <li>deadlock</li>
      </ul>
    </td>
    <td valign="top">
      Database-side logic:
      <br><br>
      <ul>
        <li>audit tables</li>
        <li>trigger functions</li>
        <li>insert/update/delete triggers</li>
        <li>generic audit trigger</li>
        <li>SQL functions</li>
        <li>PL/pgSQL functions</li>
        <li>parameterized functions</li>
      </ul>
    </td>
  </tr>
</table>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 🟢 Running locally

I run PostgreSQL in `Docker` / `OrbStack`

Connection example:

| Parameter | Value |
|---|---|
| Host | `localhost` |
| Port | `5432` |
| Database | `postgres` |
| User | `postgres` |
| Password | `postgres` |

Before running the tasks, apply the database model:

`dayXX/materials/model.sql`

Then `run` the exercise files from the corresponding `src` directory

<img src="images/delivery_pizza.png" alt="Delivery pizza" width="500"/>

<p align="center">🍕 ─────────────── 🐘 ─────────────── 🍕</p>

## 📌 Notes

This is a personal practice project 👀

The main purpose is to learn by doing, make mistakes, fix them, and slowly become less afraid of SQL 🐘

<img src="images/explain_analyze.png" alt="Explain analyze" width="500"/>