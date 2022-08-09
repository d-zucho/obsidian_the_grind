---
course: mysql
lecture: fruitTrigger.sql
---


*Primary Key* : a column, or set of columns that uniquely identifies each row.

```mysql
alter TABLE orderLine
add primary key( orderID, fruitID ), #cannot insert twice
# if you delete orderID = 24, cascade delete in orderLine
add CONSTRAINT FOREIGN key (orderID) #referential integrity
REFERENCES `orders`(orderID)
on DELETE cascade, 
# if fruit exists in orderLine, you cannot delete it from fruit
add CONSTRAINT FOREIGN key (fruitID) REFERENCES
`fruit`(fruitID) on DELETE restrict
```

==**cascade delete**== : means that if an item in "parent table" is deleted, any corresponding records/rows will be deleted in the "child table"

```ad-note
For quiz
`call fruitShared.desplayAllForeignKeys( database() )`
```


[[Intro to Triggers|Triggers]] : PLSQL code that is triggered on data manipulation

[[Constraints]] are rules that specify how foreign and primary key tables co-exist during data manipulation.

##### Triggers vs. Constraints

[[Triggers]] and [[Constraints]] both occur after some form of data manipulation

But, triggers have the entire PLSQL library available to them

