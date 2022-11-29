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

## Objects and Functions

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

