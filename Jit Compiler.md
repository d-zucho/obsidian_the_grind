---
title:  Jit Compiler
aliases:
course: javascript advanced concepts
language: javascript
tags: js
---

back:: [[Javascript - The Advanced Parts]]

# Jit Compilers

These combinations of compilers and interpreters for **"Just in time compilations"**

![[js-engine.png]]



In the [[Javascript Engine|V8 Engine]] engine, the interpreter is called the **ignition** #card #js/card 

In the [[JavaScript Engine|v8-engine]] engine, the JIT Compiler is called the ***Turbafan***

It then takes the code from the **AST** and turns it into **bytecode**, which is not as low-level as machine code, can still be interpreted by the js-engine to run program. 

The **profiler** (a.k.a **monitor**), watches the code as it runs through interpreter and makes notes on how it can be optimized.

When it sees code that can be optimized, it will then take some of that code and pass it off to the **compiler**. This is when the compiler turns some of the code into optimized machine code to run even faster. 


