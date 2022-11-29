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
-  

### Reference Counting