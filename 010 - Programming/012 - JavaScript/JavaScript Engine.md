---
type: courseNote
language: javascript
tags: js, js/javascript-engine
course: javascript advanced concepts
section: foundations
---



## JavaScript Engine
#js/js-engine 

The JS Engine helps JS write code that is asynchronous

### How it works

It takes the JS code and parses it into *tokens* analyzes what it is trying to do. #js/js-engine  # javascript/keyword

These tokens are then formed into ***ASTs***,  abstract syntax tree. #js/js-engine 

The [[Interpreter]], profiler, and [[Compiler]] then work to turn the code into optimized code for the cpu


You can run JavaScript with **the interpreter** or the **compiler**


#### Why choose one over the other?

- ***[[Compiler]]*** - program that translates one computer program into another #compiler


- ***[[Interpreter]]*** - program that directly executes instructions written in a programming language, without requiring them previously to have been compiled into a machine language program #interpreter
	- An interpreter generally uses one of the following strategies for program execution
		1. Parse the source code and perform its behavior directly;
		2. Translate source code into some efficient intermediate representation or object code and immediately executes that;;
		3. Explicitly executes stored precompiled bytecode made by a compiler and matched with the interpreted Virtual Machine
	- In interpreter also generally helps programmer find


## Inside JavaScript Engine

![[Pasted image 20221111183950.png]]


### Compiler vs Interpreter 
****
| **[[Compiler]]**                                              | **[[Interpreter]]**                                   |
| ----------------------------------------------------- | --------------------------------------------- |
| Scans Entire program first                            | Translate program one line at a time          |
| Any errors are shown at end                           | Any errors are shown line by line             |
| Main advantage - execution time                       | Slower and doesn't turn into machine code     |
| Converts source code into object code                 | No converting takes place                     |
| Doesn't require source code later for execution       | Requires source code later for execution      |
| Execution takes place after entire file is compiled   | Execution happens after every line is checked |
| Machine code is stored in disk storage                | Machine code is stored nowhere                |
| Often take lrg amnt of time for analyzing source code | Take less code for code analyzation           |
| More efficient                                        | Less Efficient                                |
| CPU utilization is more                               | CPU utilization is less                       |
| Examples: C, C++, C#                                  | Python, Ruby, Perl, MATLAB                    |
|                                                       |                                               |