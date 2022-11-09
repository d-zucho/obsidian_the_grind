---
language: react
topic: state, context
---


# Using Context API

First you need import it create a Context file and import context functionality:
```javascript
import { createContext } from 'react-context'


// Create the context object
const ProductContext = createContext()


// Create global state object as a Provider
const ProductProvider = () => {
	const [products, setProducts] = useState([
		// include all global states you want to be available
	])

	// create any functions 
	const deleteProduct = (id) => {
		...
	}

	return (
		<ProductContext.Provider
		// we MUST include what we want to be shared to other
		// components in the 'value' prop 
		value={{
			// here is where we list all states and
			// functions we want to be available
			products
			deleteProduct
		}}	
	
		>

		</ProductContext.Provider>
	)

}
```

