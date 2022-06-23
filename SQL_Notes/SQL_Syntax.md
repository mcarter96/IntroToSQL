# SQL Syntax

SQL is a declarative language, therefore, its syntax reads like a natural langage. A SQL statement begins with a verb that describes the action, for example, SELECT, INSERT, UPDATE, or DELETE. Following the verb are the subject and predicate. A predicate specifies conditions that can be evaluated as true, false, or unknown. See the following SQL statement

```SQL
SELECT
    first_name
FROM
    employees
WHERE
    YEAR(hire_date) = 2000;
```

This statement gets the first name of employees who were hired in 2000. The ```SELECT first_name```, ```FROM employees```, and ```WHERE``` are clauses in the SQL statement. Some clauses are mandatory, e.g. the ```SELECT``` and ```FROM``` clauses whereas others are optional such as the ```WHERE``` clause. Since SQL was designed specifically for non-technical people in mind, it is very simple and easy to understand. 

## SQL Commands

SQL is made up of many commands. Each SQL command is typically terminated with a semicolon. For example, the follwoing are two different SQL commands separated by a semicolon

```SQL
SELECT
    first_name, last_name
FROM
    employees;

DELETE FROM employees
WHERE
    hire_date < '1990-01-01';
```

Each command is composed of takens that can be literals, keywords, identifiers, or expressions. Tokens are separated by spaces, tabs, newlines.

## Literals

Literals are explicit values which are also known as constants. SQL provides three kinds of literals: string, numeric, and binary.

String literal consists of one or more alphanumeric characters surrounded by single quotes.

Numeric literals are the interger, decimal, or scientific notation

SQL represents binary value using the notation ```x'0000'``` where each digit is hexadecimal value

## Keywords

SQL has many keywords that have special meanings such as SELECT, INSERT, UPDATE, DELETE, and DROP. These keywords are the reserved words, therefore, you cannot use them as the name of tables, columns, indexes, views, stored procedures, triggers, or other database objects.

## Identifiers

Identifiers refer to specific objects in the database such as tables, columns, indexes, etc. SQL is case-insensitive with respect to keywords and identifiers. The following statements are equivalent:

```SQL
Select * From employees;

SELECT * FROM employees;

select * from employees;

SELECT * FROM employees;
```

## Comments

To document SQL statments, you use the SQL comments. A comment is denoted by two consecutive hypens that allow you to comment the remaining line

```SQL
-- this is a SQL comment
```

You can also use (```/* */```) for multiline notation

[Tutorial Followed](https://www.sqltutorial.org/sql-syntax/)