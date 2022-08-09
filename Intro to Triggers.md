---
language: mysql
tags: mysql/database-design
---

# Triggers

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

==PLSQL== - Procedure Language SQL 
		- MySQL with procedure language can declare variables and flow control ( if/else conditions ) #mysql/keyword #mysql/card 
		- PLSQL is ***procedure oreinted logic*** while SQL is ***declarative logic***
		- PLSQL ==procedures== are :
			- aaaa`           
---


!!! - Support for triggers varries frequntly


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
