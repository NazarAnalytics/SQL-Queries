What Can SQL do?
=================

SQL can execute queries against a database

SQL can retrieve data from a database

SQL can insert records in a database

SQL can update records in a database

SQL can delete records from a database

SQL can create new databases

SQL can create new tables in a database

SQL can create stored procedures in a database

SQL can create views in a database

SQL can set permissions on tables, procedures, and views


Some of The Most Important SQL Commands
=======================================
SELECT - extracts data from a database

UPDATE - updates data in a database

DELETE - deletes data from a database

INSERT INTO - inserts new data into a database

CREATE DATABASE - creates a new database

ALTER DATABASE - modifies a database

CREATE TABLE - creates a new table

ALTER TABLE - modifies a table

DROP TABLE - deletes a table

CREATE INDEX - creates an index (search key)

DROP INDEX - deletes an index


SQL QUERIES :
============
Selecting columns from table:-
=============================
SELECT * FROM table_name;		(here * refers to all columns)

SELECT column_name1, column_name2 FROM table_name;	(here we selecting particular columns from tabe) 

SELECT * FROM table_name WHERE id=’4’; (here we selecting all columns that belongs to id = 4)

SELECT * FROM table_name WHERE id=’4’ AND name=’ram’; (here we selecting all columns that belongs to id and also name)

SELECT * FROM table_name WHERE id=’4’ OR name=’ram’; (here we selecting all columns that belongs to id OR name)

SELECT * FROM table_name WHERE NOT id=’4’; (here we selecting all columns that not belongs to id)

SELECT DISTINCT id FROM table_name;		(id often contains many duplicate values and sometimes you only want to list the unique values.)

Insert Query:
=============
INSERT INTO table_name (column1, column2, column3) VALUES (value1, value2, value3);	(here we inserting values to the specify columns)
INSERT INTO table_name VALUES (value1, value2, value3, ...);
(the order of the values is in the same order as the columns in the table)

Order By:
=========
SELECT * FROM table_name ORDER BY id ASC; 	(selects all fields from the table, sorted ascending by the "id”)

SELECT * FROM table_name ORDER BY id DESC;	(selects all fields from the table, sorted descending by the "id")

Update Query:
=============
UPDATE table_name SET column1 = value1, column2 = value2 WHERE id=’2’;
(here we modifying the column values from table which belongs to id 2)



Delete Query:
==============
DELETE FROM table_name WHERE id=1;	(delete the all columns that belongs to id 1)

DELETE FROM table_name;		(delete all rows in table without deleting the table)
	
MIN() and MAX() Functions:
==========================
SELECT MIN(column_name) FROM table_name WHERE condition;

(MIN() function returns the smallest value of the selected column)

SELECT MAX(column_name) FROM table_name WHERE condition;

(MAX() function returns the largest value of the selected column)

SQL Like:
===========
SELECT * FROM table WHERE name LIKE 'a%';

(selects all fields with a name starting with "a")

Inner Join:
============
SELECT column_name(s) FROM table1 INNER JOIN table2 ON table1.column_name = table2.column_name;

(here INNER JOIN keyword selects records that have matching values in both tables.)

