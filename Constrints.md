---
language: mysql
tags: mysql/database-design
---

# Intro to Constraints

==Constraints==  are rules that specify how foreign and primary key tables co-exist during data manipulation #mysql/keyword
	- Mainly deal with the relationship between *foreign key* & *primary key*


```ad-info
title: Main Concept
 Rules which define the 'allowable' state of database
```

###### What happens when a record/row in a table with a foreign key, when a table with a primary key is changed? #card #mysql/card
	 One of four things can happen:
		 1. No Action -- nothing
		 2. Restrict -- stops attempted action
		 3. Cascade -- delete
		 4. Set foreign key to null









