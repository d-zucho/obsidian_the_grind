---


title:  Objects and Functions
type: courseNote
aliases:
course: javascript in detail
language: javascript
section: javascript types
tags: js


---
back:: [[012 - JavaScript]]

back:: [[Types]]

___

- [[#Objects and Functions|Objects and Functions]]
	- [[#Objects and Functions#Creating Objects|Creating Objects]]
	- [[#Objects and Functions#Adding or Modifying Properties|Adding or Modifying Properties]]




# Objects and Functions

Besides primitives, almost everything else in JS is made up of ***objects***

They are *mutable* values in JS, whose *properties* are usually accessible by using dot notation, or bracket notation: `.` or `[]` 



### Creating Objects

To create objects, we can assign a variable an empty set of  `{}` ,  or have values or **properties** in it right away

```javascript
let obj_a = {name: "Danny", age: 21}
```




### Adding or Modifying Properties

**Properties** of an object are assigned as, "*key-value pairs*" #keywords #js/keywords 

While or after declaring an object, and/or property, we can alter it using the same, dot or bracket notation. 

```ad-example
```
```javascript
obj_a.age = 31     // using dot notation
obj_a['age'] = 31  // using bracket notation
```


The value of a property, could be any variable, expression, or another object. 

```ad-note
An object's property can be assigned to a **function**. 
When this occurs, they are now called ***methods***

```



### Accessing a Property

You can access a property , again, with a dot, or bracket notation: `.` or `[]` 

```ad-example
```
```javascript
const user_age = obj_a.age   // or :
const user_age = obj_a['age']
```




## Arrays

- Kind of object that lets us make lists of items of all types. 