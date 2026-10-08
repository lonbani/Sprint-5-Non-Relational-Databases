# Sprint 5 – MongoDB: Queries and Data Analysis

## Project Overview

This project is part of the IT Academy Data Analytics program and focuses on working with MongoDB, a NoSQL document-oriented database.

The objective is to import, explore, query, and analyze a movie entertainment database using MongoDB Compass and MongoDB Shell (mongosh).

The project covers document filtering, comparison and logical operators, regular expressions, aggregation pipelines, and geospatial data visualization.

## Tools and Technologies

- **MongoDB Community Server** – Database management
- **MongoDB Compass** – Database exploration, queries, aggregation, and visualization
- **MongoDB Shell (mongosh)** – Executing MongoDB queries
- **MongoDB Query Language (MQL)** – Filtering and retrieving documents
- **Aggregation Framework** – Grouping, counting, and analyzing data

## Database Structure

The database, `sprint5_movies`, contains five collections:

| Collection | Description |
|---|---|
| `users` | Registered users and their account information |
| `movies` | Movie details, genres, release years, ratings, and awards |
| `comments` | User comments and associated movie information |
| `theaters` | Cinema locations, addresses, and geographic coordinates |
| `sessions` | User authentication sessions |

## Project Exercises

### Level 1 – Basic Queries

**Exercise 1: Data Exploration**

- Retrieve the first two comments.
- Count registered users: **185**
- Count movie theaters in California: **169**
- Identify the first registered user: **Ned Stark**
- Count comedy movies: **7,024**

**Exercise 2: Logical Operators**

Retrieve movies released in 1932 that belong to the Drama genre or are available in French.

**Exercise 3: Multiple Conditions**

Find American movies released between 2012 and 2014 with 5 to 9 award wins.

**Result:** 166 movies.

### Level 2 – Advanced Filtering and Aggregation

**Exercise 1: Regular Expressions**

Count comments associated with email addresses using the `GAMEOFTHRON.ES` domain.

**Result:** 22,841 comments.

**Exercise 2: Aggregation Pipeline**

Count movie theaters by ZIP code in Washington, DC.

Operations used:

- `$match` – Filter theaters by state
- `$group` – Group theaters by ZIP code
- `$sum` – Count theaters within each group
- `$sort` – Sort the results

### Level 3 – Advanced Queries and Geospatial Visualization

**Exercise 1: Nested Fields and Comparison Operators**

Find movies directed by John Landis with IMDb ratings between 7.5 and 8.

**Result:** 4 movies.

**Exercise 2: Geospatial Data**

Visualize movie theater locations on an interactive map using MongoDB Compass Schema Analysis.

## Key Concepts Practiced

- NoSQL document-oriented databases
- Collections, documents, and nested fields
- MongoDB Query Language (MQL)
- `find()`, `findOne()`, `countDocuments()`, `sort()`, and `limit()`
- Comparison operators: `$gte`, `$lte`
- Logical operators: `$or`
- Regular expressions: `$regex`, `$options`
- Aggregation pipelines: `$match`, `$group`, `$sum`, `$sort`, `$count`
- Field projection
- Geospatial data exploration

## Project Documentation

The complete exercise solutions, including MongoDB queries and screenshots of execution results, are available in:

**[Task S5.01. Queries with MongoDB.pdf](Task%20S5.01.%20Queries%20with%20MongoDB.pdf)**

## Learning Outcomes

Through this project, I gained practical experience in querying and analyzing semi-structured data using MongoDB.

I also strengthened my understanding of the differences between relational databases and NoSQL systems, particularly in data modeling, filtering, aggregation, and geospatial analysis.

The project demonstrates how MongoDB can support analytical queries and data exploration within a document-oriented database environment.
