# IMDB
Analyzed IMDb movie data using SQL to extract insights on top-rated films, popular genres, and prolific directors. Applied advanced SQL techniques including joins, subqueries, and aggregations to uncover trends in movie ratings and production over time.

# 🎬 IMDb SQL Project

This project involves analyzing IMDb movie data using SQL to uncover trends and insights related to movie ratings, genres, and directors.

---

## 📘 Project Overview

The goal of the project is to extract meaningful insights from a relational IMDb database by writing and executing SQL queries. The analysis includes identifying top-rated movies, most active directors, genre popularity, and yearly trends in film production.

---

## 🧰 Tools & Technologies

- SQL (Structured Query Language)
- MySQL / SQLite / PostgreSQL *(choose your DBMS)*
- MySQL Workbench / DBeaver / Jupyter + SQLite *(choose your interface)*

---

## 📊 Key Queries & Insights

- 🎥 Top 10 highest-rated movies
- 🧑‍🎬 Most prolific directors
- 📈 Yearly trend of movie releases
- 🌟 Average rating by genre
- 🧮 Use of JOINs, GROUP BY, HAVING, subqueries, and aggregate functions

---

## 💡 Sample Query

```sql
SELECT m.title, r.rating
FROM movies m
JOIN ratings r ON m.movie_id = r.movie_id
ORDER BY r.rating DESC
LIMIT 10;
