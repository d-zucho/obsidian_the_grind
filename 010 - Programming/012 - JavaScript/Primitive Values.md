---


title:  Primitive Values
type: courseNote
aliases:
course: javascript in detail
language: javascript
section: 
tags: js


---
back:: [[012 - JavaScript]]

back:: [[Types]]


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


### Symbol #keywords #js/keywords 

- Allows us to include unique identifiers in code
- often used when we need to have a value in code that is *unique* to a program

```ad-caution
For **symbol**, we don't use the `new` kewyword because it does not have a contructor
```
