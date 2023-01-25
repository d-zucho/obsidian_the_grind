---


title:  React Props
type: courseNote
alias:
course: Modern React with Redux
teacher: stephen grider
language: react
section: 
tags: react


---
back:[[015 - React]]

## Some general rules regarding *[[Props]]*

1. All prop names follow camelCase capitalization
2. Number attributes use curly braces
3. Booleans of "true" can be written with just the property name
4. The 'class' attribute becomes 'className'
5. In-line styles are provided as objects


#### Example:

```jsx
function App() {
  return (
    <div class="wrapper">
      <textarea
        read-only="true"
        maxLength="3"
        spellcheck="true"
        style="background-color: gray;"
	  />
    </div>
  )
}
```

**Becomes**

```jsx
function App() {
  return (
    <div className="wrapper">
      <textarea
        readOnly
        maxLength={3}
        spellCheck
        style={{"background-color: gray;"}}
	  />
    </div>
  )
}
```






