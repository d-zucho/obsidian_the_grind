---
language: react, jsx
---

# Set Form Input as State

When we use an `<input>` and want to use what is entered as the `component's` `state`, first connect the input to state with a `useState()` call.

In the `input` attribute sction, connect a :
`onChange` handler `handleTextChange`

```jsx

// FeedbackForm Component
const FeedbackForm = () => {

	const [text, setText] = useState('')  
	
	const handleTextChange = (e) => {
	
		// set 'text' state as input text with event handler
		setText(e.target.value)
	}

	return (
		<Card>
		
			<form>
			
				<h2>How would you rate your service with us?</h2>
				
				
				<div className='input-group'>

					<!-- input field where any changes will be connected
						 to component state through handleChangeText function	
					 -->
					<input
						placeholder='Write your review here...'
						type='text'
						name='review-text'
						id='review-text'
						onChange={handleTextChange}
						value={text}
					/>
					<button>Submit</button>
				</div>
			</form>
		</Card>
		)
	}
```
