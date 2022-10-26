---
language: react, redux
topic: redux, redux-toolkit, react-redux, state
tags: react/redux, react/state-management
---
back:: [[015 - React]]

### Lets start with a mock folder structure
	|- app
	-| - src
		-| - features
				*todoSlice.js


**In `todoSlice.js` we will start with creating out global state**

```js
import { createSlice } from '@reduxjs/toolkit'

// where we start defining the global state
const initialStatew = {
	todoList: []
}

const todoSlice = createSlice({
	name: 'todos',
	initialState,
	// reducers are functions that modify the state
	redicers: {
	    saveTodo: (state, action) => {
	    // state is the global state, action is the payload which is the data we want to save
	       state.todoList.push(action.payload)  // push the payload to the todoList array
	    }
	}
})
```
