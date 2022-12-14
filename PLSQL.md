---
language: mysql, plsql
tags: mysql, mysql/plsql
---

- [[#What is PLSQL|What is PLSQL]]
- [[#Advantages of PLSQL|Advantages of PLSQL]]
- [[#Syntax|Syntax]]


# PLSQL

## What is PLSQL

==PLSQL== is a procedural language designed to work with [[SQL - Database Design|SQL]] statements 
 - Developed by Oracle in 90s
- #### PLSQL Variables

==PLSQL variables== :
 - type must match MySQL field types
 - Can only declare onve variable at a time
 - Variable declarations must be at bginning of PLSQL block
* Delimeter required when declaring variables
yout

* Variable with '@' declare "session variables"


## Advantages of PLSQL

-   SQL is the standard database language and PL/SQL is strongly integrated with SQL. PL/SQL supports both static and dynamic SQL. Static SQL supports DML operations and transaction control from PL/SQL block. In Dynamic SQL, SQL allows embedding DDL statements in PL/SQL blocks.
-   PL/SQL allows sending an entire block of statements to the database at one time. This reduces network traffic and provides high performance for the applications.
-   PL/SQL gives high productivity to programmers as it can query, transform, and update data in a database.
-   PL/SQL saves time on design and debugging by strong features, such as exception handling, encapsulation, data hiding, and object-oriented data types.
-   Applications written in PL/SQL are fully portable.
-   PL/SQL provides high security level.
-   PL/SQL provides access to predefined SQL packages.
-   PL/SQL provides support for Object-Oriented Programming.
-   PL/SQL provides support for developing Web Applications and Server Pages.


## Syntax

PL/SQL is a procedural, block-structured langues == is written in blocks of logical code

**Each block consists if 3 parts** :

| Step | Section / Description                                                                                                                                                                              |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | **Declarations** - starts with DECLARE; opetional section and defines all variables, cursors, and other elements                                                                                   |
| 2    | **Executable Commands** - Mandatory Section; Begins with keywords *Begin* and *End*. Consists of executable PLSQL statements. SHould have at least one executable line; can even be a NULL command |
| 3    | **Exception Handling** - Section starts with `Exception`. This optional section contains **exceptions**. Section contains exception(s) that handle errors in the program.                          |

```mysql
# This code states that if customer tries to order an amount that is greater than available, change customer order amount to amount available

DECLARE desired int; # desited is what we want to snd to cutomer
DECLARE orderLineRows CURSOR FOR
select fruitID, quantity from orderLine
where orderLine.orderID = old.orderID;
OPEN orderLineRows;
select FOUND_ROWS() ubti riwCiybt;
while rowCount > 0 do
	FETCH orderLineRows into fID, desired;
	set available = (select ifnull(quantity, 0) from fruitView where fruitID = fID);
	IF (desired > available) then
		#remember orderID, fruitID is the primary key for orderLine
		update orderLine set orderLine.quantity = available
		where orderLine.orderID = new.orderID and orderLine.fruitID = fID;
		set desired = available;
	END IF; call updateInventory( fiD, desired );
	set rowCount = rowCount - 1;
END while;
CLOSE orderLineRows
```







