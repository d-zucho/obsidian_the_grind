---
language: react, jsx
---

# Set Form Input as State

When we use an `<input>` and want to use what is entered as the `component's` `state`, first connect the input to state with a `useState()` call.

```javascript

// FeedbackForm Component
const FeedbackForm = () => {

const [text, setText] = useState('')  // conn

const handleTextChange = (e) => {

// set 'text' state as input text

  

setText(e.target.value)

}

  

return (

<Card>

<form>

<h2>How would you rate your service with us?</h2>

{/* @todo - rating select component */}

<div className='input-group'>

<label htmlFor='review-text' />

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
