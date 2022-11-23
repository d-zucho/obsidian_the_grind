---


title:  Clearing Input Field in React
alias:
topic: clearing input fields in react 
language: react
tags: react

---
back:: [[Youtube Todo ( Dev GB )]]



```javascript

import {useState} from 'react';

const App = () => {
  const [firstName, setFirstName] = useState('');
  const [lastName, setLastName] = useState('');

  const handleSubmit = event => {
    console.log('handleSubmit ran');
    event.preventDefault(); // 👈️ prevent page refresh

    // 👇️ clear all input values in the form
    setFirstName('');
    setLastName('');
  };

  return (
    <div>
      <form onSubmit={handleSubmit}>
        <input
          id="first_name"
          name="first_name"
          type="text"
          onChange={event => setFirstName(event.target.value)}
          value={firstName}
        />
        <input
          id="last_name"
          name="last_name"
          type="text"
          value={lastName}
          onChange={event => setLastName(event.target.value)}
        />

        <button type="submit">Submit form</button>
      </form>
    </div>
  );
};

export default App;

```


