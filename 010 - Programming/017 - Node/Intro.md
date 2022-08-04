## Creating & Exporting Your Own Modules

- When creating your own files/modules in node, if you want these to be available accross your program, you need to ***export them*** #node/modules
- 
```javascript

let hello = () => {
	console.log('hello')
}

module.exports = hello;
```


### Using Your Own Modules in Other files

To use the modules you created in other files, you need to ***import*** them
```node
const hello = require('.Hello.js')
```



```ad-hint
When you have 3 functions in the same file, and we only want 2 of them:


>	let foo = function() {...}
>	let bar = function() {...}
>	let baz = function() {...}

>	exports.foo = foo
>	exports.bar = bar


	// Then in the other file, we would call them as such:
	const myMod = require('/myModule')


>	myModule.foo()
>	myModule.bar()


```



