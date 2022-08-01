---
language: react, jsxp
---

# handleClick To Delete Item in List


Many times items are `mapped` through to add individual `components` to a page.
To do this, you have to add the function as a *prop* to the *item component*

#### Example:

```javascript

const myList = [
	{
		id: 1,
		text: "some text"
	},
	{
		id: 2,
		text: "some other text"
	}
	...
]


// component where we will map throught the list
function listComponent(myList) {
	// first use .map to iterate through list
	myList.map(item => (
		// add a the handleClick function as a prop VV
		<ListItemComponent aClickFunction={handleClick} />
	
	
	))
	
}
```
