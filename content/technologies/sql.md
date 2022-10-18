---
title: "SQL"
date: 2022-10-13T11:26:45+08:00
tags:
- technologies
---

Abbreviated term for Structured Query Language, often pronounced as 'sequel'. Used as a language used in [[technologies/databases|databases]] to query for data according to specified instructions by the language. Used to create, query, and update relational databases.

# Keywords

| Keyword | Description |
|:-:|:-|
| `SELECT` | Selects the given fields from a database |
| `SELECT ... WHERE` | Selects the given fields from a database, provided the conditions provided are true |
| `FROM` | Specifies which table should data be retrieved from |
| `AS` | Aliasing a field name in the query |
| `DISTINCT` | Filters a field and removes duplicate values |
| `CREATE VIEW` | Creates a new view |
| `ORDER BY ... ASC` or `ORDER BY ... DESC` | Sorts a field in ascending or descending order |
| `LIKE` | Performs pattern match searching |

# Logical operators

- `AND`
- `OR`
- `IN`
- `NOT`
- `IS`

# Terminologies

| Term | Definition |
| :-:|:-|
| Result set | The produced data after processing a query |
| View | A table that is a saved result set |
| Virtual table | Not a table in the database, but the query code is saved instead |

# Data types
Often [[technologies/data-typing|data typed]] and store a particular piece of required information; common data types include:

| Data type | Used for |
|:-:|:-|
| `VARCHAR` | A variable-length string; can be used for anything ranging from an individual character to a string of thousands of characters. |
| `INTEGER` or `INT` | A medium-sized integer (32-bits) |
| `BOOL` | Boolean |

# Best practices
- End off queries with a semicolon to denote that the query is complete
	```sql
	SELECT name
	FROM patrons;
	```