## JavaScript Engine
#javascript/js-engine 

The JS Engine helps JS write code that is asynchronous

### How it works

It takes the JS code and parses it into *tokens* analyzes what it is trying to do. #javascript/js-engine  

These tokens are then formed into ***ASTs***,  abstract syntax tree. #javascript/js-engine 

The interpreter, profiler, and compiler then work to turn the code into optimized code for the cpu


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

