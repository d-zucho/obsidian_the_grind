---


title:  Calling from API with fetch()
type: codingNote
alias:
topic: API Calls & async await 
language: react
tags: react, js/api-call, js/async-await

---

back: [[010 - Programming/015 - React/_index_]]



## Calling from API with fetch()


When we have our getter function to an API, we **always** need to make sure we set it up as an *async await* call.

>[!example]
>```javascript
>const getSomeData = async() => {
>	const getInfo = await fetch('www.someSiteNameHere')
>	const data = await getInfo.json()
>	// now our readable information will be stored in data
>}
>
>```





