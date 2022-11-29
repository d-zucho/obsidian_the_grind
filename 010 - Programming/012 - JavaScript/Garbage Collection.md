---


title:  Garbage Collection
aliases:
course: javascript advanced concepts
language: javascript
section: foundations
tags: js, garbage-collection


---
back:: [[012 - JavaScript]]

back:: [[Javascript - The Advanced Parts]]

---

When javascript allocates memory, automatically, when function is run and an object is created within function, as it is finished and we no longer need a function-created-object, that object will be deleted from memory.

Garbage collector frees memory on the heap, preventing *memory leaks* - when memory gets too big and reaches maximum size


## 2 Main Types of Garbage Collection

### Mark Removing

- <mark style="background: #FFF3A3A6;">most common method</mark>

**Quick overview/summary of steps:

- When a variable enters the executing environment, it is marked as *"entering the environment"* and will remain in memory until it is no longer in the environment. It is then marked as *"leave the environment"*.

- Garbage collector than comes and 'marks', or 'tags', all variables that are stored in memory. 

- It then removes the mark from any variable in the environment or referenced by variables in the environment. 

- Any other variable in memory is now ready to be deleted -- leading to space in memory being cleared. 






### Reference Counting