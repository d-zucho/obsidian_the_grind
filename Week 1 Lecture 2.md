---
course: Intro to Computer Science
type: assignment
title: Week 1 Lecture Exercise 2
status: notDone
due: 1/24/23
submitted: late
tags: assignment
---

- Single Binary digit = **bit**
- It takes 8 bits to store a single character
- *8 Bits = 1 Byte*


**ASCII** - American Standard Code of Information Interchange

Initally each code consisted of a 7-bit code, but then turned into **extended version which is a 8 bit**

This is sufficient for English, buit not for Foreign Languages because of special characters


**Unicode** - developed for international use

Unicode uses (65,536) or 2^16
___

# The Decimal System

- Base 10
Brought to us by the hindus, we adopted it in 1200 AD

- Decimal makes it easy to deal with large quantities with relatively few digits
- Makes use of *10 digits ( 0-9 )*
- These symbols have a "*place value*" or *positional concept* which allow us to represent any whole number

## Numbers & the machione

- We think in decimal (BASE 10)
	- 0, 1, 2, 3, 4, 5, 6, 7, 8, 9

- Computers think in Binary (Base 2)
	- 0 and 1

- Since *binary can get long*, it is easier to use **octal** (base 8), or **hexadecimal** (base 16) equivalents


# Positional Numbering Systems

Position **MATTERS** in decimal

> 352
> 3 represents 10^2
> 5 represents 10^1
> 2 represents 10^0
> --
> This means 3 * 10^2 + 5 * 10^1 + 2 * 10^0
> 


Rules for Positional Notation

1. Number of distinct symbols equals the base
2. Largest value represented by 1 symbol, is one less than the base
	1. for base 10, this is 9
3. Each alue of a number is multiplied by the base raised to the appropriate power relative to its position