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