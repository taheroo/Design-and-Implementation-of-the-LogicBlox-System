# Design and Implementation of the LogicBlox System

This is the first time I will try to understand a research paper ! </br>
I will try to ask question about things I didn't understand and try to make some research to understand them.

## LogicBlox

LogicBlox's primary product is what we call a smart database. </br>
It's an active cloud database that has much </br>
of the business logic that one would normally need to write in a traditional </br>
imperative language running on separate machines down in the database. </br>
So that when data are added to the database, </br>
these business rules kick in and update views automatically. </br>
It specializes in doing really large-scale analytics and </br>
applications that are kind of a hybrid between transactional and analytic, </br>

Source: ["LogicBlox"](https://www.youtube.com/watch?v=8d9FY6MHO-c&ab_channel=Udacity)

## ABSTRACT

```text
The LogicBlox system aims to reduce the complexity of software
development for modern applications which enhance and automate
decision-making and enable their users to evolve their capabilities
via a “self-service” model. Our perspective in this area is informed
by over twenty years of experience building dozens of missioncritical enterprise applications that are in use by hundreds of large
enterprises across industries such as retail, telecommunications,
banking, and government. We designed and built LogicBlox to be
the system we wished we had when developing those applications.
In this paper, we discuss the design considerations behind the
LogicBlox system and give an overview of its implementation,
highlighting innovative aspects. These include: LogiQL, a unified
and declarative language based on Datalog; the use of purely functional data structures; novel join processing strategies; advanced
incremental maintenance and live programming facilities; a novel
concurrency control scheme; and built-in support for prescriptive
and predictive analytics.

```

Resume:
The LogicBlox system aims to reduce the complexity of software </br>
development for modern applications. </br>

What is Datalog ?

Datalog is a declarative logic programming language. </br>
It is often used as a query language for deductive databases.

What is Declarative programming ?

- In an imperative programming language, a program specifies how to solve a problem.
- In a declarative language, a program specifies what needs to be solved :
  - The language itself needs to provide a way to find the solution
  - Sometimes called rule-based languages

Examples

- Prolog (logic programming)
- MYCIN (Expert system)
- SQL (databases)

What is 'Deductive database' ?

A deductive database is a database system that can make deductions based on rules and facts stored in the database. </br>
Datalog is the language typically used to specify facts, rules and queries in deductive databases.

What is LogiQL ?

LogiQL is a programming language for accessing logic databases

What does it mean 'join processing strategies' ?

If you are familiar with SQL, you are probably very familiar with using joins between tables in creating SQL queries. A join occurs any time the SQL Server Query Optimizer has to compare two inputs to determine an output. The join can occur between one table and another table, between an index and a table, or between an index and another index (as described previously, in the section, “Index Intersection”).

The SQL Server Query Optimizer uses three primary types of join strategies when it must compare two inputs: nested loops joins, merge joins, and hash joins. The Query Optimizer must consider each one of these algorithms to determine the most appropriate and efficient algorithm for a given situation.

Source: https://www.oreilly.com/library/view/microsoft-sql-server/9780133408539/ch31lev2sec11.html

What does it mean 'purely functional data structures' ?

What does it mean 'Incremental Maintenance' ?

What does it mean 'Transaction Repair' ?
