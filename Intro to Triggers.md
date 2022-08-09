---
language: mysql
tags: mysql/database-design
---



- [[#Triggers|Triggers]]
			- [[#Triggers are ***PLSQL***  code that is 'triggered' on data manipulation|Triggers are ***PLSQL***  code that is 'triggered' on data manipulation]]
	- [[#Triggers#PLSQL|PLSQL]]
		- [[#PLSQL#Trigger Syntax - Create a trigger|Trigger Syntax - Create a trigger]]



## Triggers

Triggers aid in prohibiting bad database states 

They are ***PLSQL*** code that is 'triggered' on data manipulation

Triggers are associated with **specific tables**
___
```ad-summary
title: Key Point
Triggers occure before OR after data change/manipulation.

Triggers are associated with *tables*
```
___

##### Triggers are ***PLSQL***  code that is 'triggered' on data manipulation

### PLSQL 

==PLSQL== - Procedure Language SQL   
		- MySQL with procedure language (PLSQL) can declare variables and flow control ( if/else conditions ) #mysql/keyword #mysql/card 
		- PLSQL is ***procedure oreinted logic*** while SQL is ***declarative logic***
		- PLSQL ==procedures== are :
			- accept input
			- block of code that executes as a group
			- can declara variables
			-  can use sql statements in code
			- can use flow control


#### PLSQL Variables

==PLSQL variables== :
 - type must match MySQL field types
 - Can only declare onve variable at a time
 - Variable declarations must be at bginning of PLSQL block
* Delimeter required when declaring variables
yout

* Variable with '@' declare "session variables"
	* New sessions occur on each page load
 

```ad-danger
title: Warning
Triggers do NOT work with *views*
```



#### Trigger Syntax - Create a trigger
To create a trigger:
```mysql
create trigger [triggerName]
[before | after]
[update | delete | insert]
on [tableName]

```


#### Cursors

A ==cursor== is an object that helps us enumerate over and process the individual rows returned by a query