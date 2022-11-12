---
type: courseNote
language: javascript
tags: javascript, javascript/compiler, javascript/javascript-engine, 
course: javascript advanced concepts
section: foundations
---

back::[[JavaScript Engine]]

## Compiler vs Interpreter 


| **[[Compiler]]**                                      | **[[Interpreter]]**                           |
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