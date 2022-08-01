back: [[015 - React]]



# State 


React's state helps make website **interactive**


## Purpose 


> In simple terms, state help's information change 

It ***observes*** website to wait for changes, which then trigger some kind of action; this could be: 
	- input being typed
	- radio buttons / checkboxes
	- etc.

Whatever info is recorded, is then stored in the state object, which can then be passed to other components as a prop.


## How to set it up

###### Syntax - **useState() Hook**


```javascript
const [day, setDay] = useState('')

// this syntax is explained with:
// [stateVariable, setState function] = useState('starting value of stateVariable')
```


## 2 Types of State
1. Compnent Level State
	- State simply dealing with the component it is in
1. App Level State
	- State that would be used/accessible by multiple, if not all, components



