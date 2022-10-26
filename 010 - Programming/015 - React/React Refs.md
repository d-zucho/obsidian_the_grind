---
language: react
topic: ref
---

```ad-info
title: What are ***Refs***

Refs provide a way to access *DOM* nodes or React elements created in the render method
```

Typically, props are only way that parent ocmponents interact with children. 
	*Example* -- To modify a child, you re-render it with new props


## When to use Refs:

- Managing focus, text selection, or media selection
- Triggering imperative animations
- Integrating with third-party DOM libraries


```ad-warning

Avoid using Refs for anything that can be done declaritively
```

***Usually*** you cant use refs in class components, but you CAN use them in functions when youy are refering to a DOM element or a class component