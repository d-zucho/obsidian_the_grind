---
topics: refresher, syntax
language: javascript
---
 back:: [[012 - JavaScript]]


# Spread & Rest Operator


- [[#Spread Operator|Spread Operator]]
	- [[#Spread Operator#When is it Used?|When is it Used?]]
			- [[#Example with Array:|Example with Array:]]
			- [[#Example with Object:|Example with Object:]]


The `spread` and `rest` operator both have the same syntax:: `...`
<!--SR:!2022-08-16,3,250-->


The **difference**, is how it is used, which will determine if it is a spread or rest operator.

## Spread Operator

When using it  as the ==spread== operator, you end goal is : #card #javascript/card 
	to pull out elements of a list or properties out of an object and "spread" them out, without having to recode every line and property.
<!--SR:!2022-08-16,3,250-->

### When is it Used?
The spread operator is often used when changing `state` in react. Why? #card  #react/card #javascript/card 
	- Since `state` is immutable, when we want to make a change, we do it by "copying" or "piulling out" the properties of the previous state, and adding new values or changing old to the new values.

##### Example with Array:
```javascript
const oldArray = [1, 2, 3]

// Add oldArray valus to new array with spread operator
const newArray = [...oldArray, 4, 5, 6] 
```

##### Example with Object:
```JavaScript
// changing values in one object would use:
const oldObject = {
	bane: 'Danny'
}

const newObject = {
	...oldObject,
	age: 31
}
```

What is **rest operato** #review-later 
