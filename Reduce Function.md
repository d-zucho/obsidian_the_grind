---
language: javascript
---
back: [[012 - JavaScript]]

###### [mdn docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)

# Reducer Functions


Main goal is to take an array and apply an element  "*reduce*" it down to a signle value

Has **2 parameter** : 
		1. `accumulator`
		2. `currentValue`

```javascript
// example
[3, 5, 7, 9, 11].reduce((accumulator, currentValue) => {
	return accumulator + currentValue
})

// output:  35
```

```ad-check
title: Explanation
collapse: open
![[CleanShot 2022-08-21 at 12.47.56.png]]

```

