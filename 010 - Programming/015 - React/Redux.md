---
language: react, redux
topic: redux, redux-toolkit, react-redux, state
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

const initialStatew = {
	todoList: []
}

const todoSlice = createSlice({
	name: 'todos',
	initialState,
	redicers: {
	saveTodo: (state, action) => {
	}
	}
})
```
