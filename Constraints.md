---
language: mysql
tags: mysql/database-design
---

- [[#Referential Integrity|Referential Integrity]]

# Intro to Constraints



==Constraints==  are rules that specify how foreign and primary key tables co-exist during data manipulation #mysql/keyword
	- Mainly deal with the relationship between *foreign key* & *primary key*


```ad-info
title: Main Concept
- Rules which define the 'allowable' state of database
- Work only with Foreign Keys
```

EXAMPLE :
 the type definitions can be considered restraints
	 - price  decimal(5, 2); limited to 0.00 - 999.99


What happens when a record/row in a table with a foreign key, when a table with a primary key is changed? #card #mysql/card
	 One of four things can happen:
		 1. No Action -- nothing
		 2. Restrict -- stops attempted action
		 3. Cascade -- delete
		 4. Set foreign key to null


To add a constraint, use the syntax:
	- `alter table [tableName] add [...constraint name]`

## Referential Integrity

==Referential Integrity== means  to maintain integrity by making sure the foreign key always references to the primary key #mysql/keyword #mysql/referencial-integrity


```ad-example
title: Example - Referential Integrity Violation
Referential Integrity **Violation** occurs when a foreign key points to a non-existent primary key
```

***Enforcing Referential Integrity*** :
	- select storage engine that supports referential integrity
		- storage engine = software component that manages the storage of data
	-  add foreign key constraint

##### Referential Integrity Violation Syntax Example

<mark style="background: #FFFFFF">Syntax Example</mark> 
```mysql
# checks for violation of referential integrity
SELECT * from `inventoryQuantity`
LEFT JOIN `fruit`
on fuit.fruitID = inventoryQuantity.fruitID
WHERE fruit.fruitID IS NULL;
```

<mark style="background:#FFFFFF">Helooooo</mark>