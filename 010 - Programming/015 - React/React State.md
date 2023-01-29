---
type: codingNote
language: react
topic: React State
tags: react, react/state, 
---


back: [[010 - Programming/015 - React/_index_]]



```ad-abstract
title: Ways To Pass Data To/From Components
1. Render Props
2. Context API
3. React Hooks(useContext API)
4. React-Redux / Redux
5. Other state management libraries (i.e. XState, MobX)
```


# State 


React's state helps make website **interactive**

- It is a structure that ==keeps track of how data changes over time== in your application. 

```ad-important
When state object changes, the component re-renders
```


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



## Local State & Global State
