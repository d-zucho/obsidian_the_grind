---


title:  Types
type: courseNote
aliases: ["types", "js types"]
course: javascript in detail
language: javascript
section: javascript types
tags: js


---
back:: [[012 - JavaScript]]

back:: [[Javascript in Detail - From Beginner to Advanced]]


# Types
---

**_Types_** can be categorized in 2 different categories:
1. _Primitive Values_
2. _Objects and functions_


## Primitive Values

		- Boolean
		- Number
		- Null
		- Undefined
		- String
		- Symbol

- **Immutable** - in the way that a primitive itself cannot be modified, but new primitives can be created, and those values are assigned to variables # js/primitive-values
- They are **read only**.
	- For example:
		- if we try to access a string with bracket notation, we can read out the letter at the index, however, we can NOT change that letter.
		- We can of course assign the variable a new value, but we can not change the existing value.




### Null #keywords #js/keywords 

- Null - Represents, literally, nothing. Nothingness. 

>[!note]
>Only One value for null: `null`


### Undefined #keywords #js/keywords 

- Undefined - Value assigned to variables who do not yet have a value 

>[!note]
>Only One value for undefined: `undefined`



### Number #keywords #js/keywords 

- Number - Consist of all numeric values -- decimals (floats) and regular numbers 

	#### Using e notation
	- Can initialize a number using '*scientific notation*']]
	 ```javascript
	 let num1 = 2e-3 // 0.002
	 let num2 = 10e5 // 1000000
	```


>[!note]
>There are also special numeric values in the number type:
> - Infinity
> - -Infinity
> - NaN



### String #keywords #js/keywords 

- Value consisted of characters surrounded in quotes
- Can be *single* quotes, *double* quotes, or *backticks*

>[!example]
>For backticks, using template strings consists of:
>```javascript
>let name = 'Danny'
>console.log(`My name is ${name}`)
>```


Symbol