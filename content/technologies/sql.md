---
title: "SQL"
date: 2022-10-13T11:26:45+08:00
tags:
- technologies
---

- Abbreviated term for Structured Query Language, often pronounced as 'sequel'
- Used as a language used in [[technologies/databases|databases]] to query for data according to specified instructions by the language
- Creating, querying, and updating relational databases

# Keywords
| Keyword | Description |
|:-:|:-|
| `SELECT` | Selects the given fields from a database |
| `FROM` | Specifies which table should data be retrieved from |
| `AS` | Aliasing a field name in the query |
| `DISTINCT` | Filters a field and removes duplicate values |
| `CREATE VIEW` | Creates a new view |

# Terminologies
| Term | Definition |
| :-:|:-|
| Result set | The produced data after processing a query |
| View | A table that is a saved result set |
| Virtual table | Not a table in the database, but the query code is saved instead |

# Best practices
- End off queries with a semicolon to denote that the query is complete
	```sql
	SELECT name
	FROM patrons;
	```