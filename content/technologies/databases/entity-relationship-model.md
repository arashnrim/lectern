---
title: "Entity-relationship model"
date: 2022-11-01T09:21:57+08:00
tags:
- technologies
- databases
---

A database visualisation model that describes interrelated things of interest in a specific domain of knowledge. Provides a detailed and logical representation of the data in a database.

# Terminologies

| Term | Definition |
|:-:|:-|
| Simple/Atomic attribute | An attribute that cannot be further divided into smaller attributes |
| Composite attribute | An attribute that is made up of multiple components, each with an independent existence |
| Single-valued attribute | An attribute that holds only a single value for a single entity (e.g., name, gender, ID) |
| Multi-valued attribute | An attribute that holds multiple values for a single entity (e.g., phone numbers, qualifications) |
| Derived attribute | An attribute that represents a value derivable from the value of related attributes | 

# Symbols

| Symbol | Representation |
|:-:|:-|
| Rectangle | Entity (singular) |
| Concentric rectangle | Weak entity (singular) |
| Oval | Simple/Composite single-valued attribute; underlined attributes represent primary keys |
| Concentric oval | Single/Composite multi-valued attribute |
| Dotted oval | Derived attribute |
| Diamond | Relationship (verb) |

| Line | Representation |
|:-:|:-|
| Single line | Partial/Optional participation |
| Double line | Total/Mandatory participation |

# Relationships

## Degrees of relationships
Relationships can have different degrees to show in an ER model. Common degrees include the:
- unary (one) degree;
- binary (two) degree; and
- ternary (three) degree.

### Unary relationships
Represents the relationship between instances of a single entity. Also known as a recursive relationship.

- It is important to assign a role name that signifies the function a participating entity plays in each relationship; this allows you to distinguish the meaning of each participation

### Binary relationships
Represents the relationship between instances of two entities. Is the most common type of relationship encountered in data modelling.

### Ternary relationships
Represents the relationship among instances of three entities.

## Constraints
Relationships can be constrained such that only certain cases are valid in a database. This helps to plan out a database in greater detail.

### Cardinality ratio
Refers to the number of instances of an entity that can be associated with an instance of another entity. The three most commonly-used cardinality ratios used in databases include:
- one-to-one (1:1) relationship;
	- example: one staff member supervising one branch
- one-to-many (1:M) relationship; and
	- example: one book publisher publishing many books
- many-to-many (M:N) relationship.
	- the 'N' is used to differentiate the letters, but still means many. Can be ignored (don't need to change)
	- example: many students taking many subjects

### Participation
Specifies whether the existence of an entity depends upon it being another entity through the relationship. Shown in the ER diagram as different strokes of lines connecting entities and relationships.

Generally has two participation constraints:
- partial/optional participation, where instances of an entity are related to instances of another entity through the relationship, but not necessarily all; and
- total/mandatory participation, where instances of an entity must be associate with an instance of the related entity.