---


title:  Variable Mutation
type: courseNote
aliases:
course: javascript in detail
language: javascript
section: Values & Variables
tags: js


---
back:: [[012 - JavaScript]]

back:: [[Javascript in Detail - From Beginner to Advanced]]

---
# Mutated Values

Variable mutation is simply *reassigning* a variable to another value. 
- This can just be done using the assignment operator ('=')
```javascript
var a = 5
var a = 20
```


 When we do this, we **mutate** our variable


# Copy Values

We can use *values* through *variables* and assign them to other *variables*.

We do this by assigning a variable to the other variable directly. 


#### Example:

```javascript
var variable_1 = 100; 
var variable_2 = 200; 
var variable_3 = variable_1; // assign to value of variable_1 console.log("variable_1: ",variable_1); // print variable_1 value console.log("variable_2: ",variable_2); // print variable_2 value console.log("variable_3: ",variable_3); // print variable_3 value 

variable_1 = variable_2; // assign to value of variable_2 
variable_2 = 500; 
console.log("Values after update:"); 
console.log("variable_1: ", variable_1); // print variable_1 value
console.log("variable_2: ", variable_2); // print variable_2 value
console.log("variable_3: ", variable_3); // print variable_3 value
```

![[CopyValuesExample.png]]