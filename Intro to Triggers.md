---
language: mysql
tags: mysql/database-design
---

# Triggers

Triggers aid in prohibiting bad database states 

They are ***PLSQL*** code that is 'triggered' on data manipulation


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

---


!!! - Support for triggers varries frequntly


```ad-warning
Triggers do NOT work with *views*
```



#### Trigger Syntax
To create a trigger:
```mysql
create trigger [triggerName]
[before | after]
[update | delete | insert]
on [tableName]

```
