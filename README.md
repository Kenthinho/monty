# Monty Bytecode Interpreter

### Documentation

## Installation
- compile with the following:
  - gcc -Wall -Werror -Wextra -pedantic *.c -o monty
  - usage: ./monty <filename>
    - filename should contain the operators
    - One operator per line
    - spaces and newlines are ignored


## Monty Language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like python).
It relies on a unique stack, with specific instructions to manipulate it. The goal of this project 
is to create an interpreter for Monty ByteCodes files.

- monty.h - contains all the structure and prototype
- main.c - main function for monty interpreter


## Operator Instruction
- push - pushes value to stack
  - usage: push 123
- pall - prints everything on the stack LIFO
  - usage: pall
- pint - prints the top value of the stack
  - usage: pint
- add - adds the top two elements of the stack
  - usage: add
- sub - subtracts the top element of the stack from the second top element of the stack
- swap - swaps the top two elements of the stack
  - usage: swap
- pop - removes the top element of the stack
  - usage: pop
- nop - doesn't do anything
  - usage: nop
- div - divides the second top element of the stack by the top element of the stack
  - usage: div
- mul - multiplies the second top element of the stack with the top element of the stack
  - usage: mul
- mod - computes the rest of the division of the second top element of the stack by the top element of the stack
  - usage: mod
- pchar - prints the char at the top of the stack, followed by a new line
  - usage: pchar
- pstr - prints the string starting at the top of the stack, followed by a new line.
  - usage: pstr
- rotl - rotates the stack to the top. The top element of the stack becomes the last one, and the second top element of the stack becomes the first one
  - usage: rotl
- rotr - rotates the stack to the bottom. The last element of the stack becomes the top element of the stack
  - usage: rotr
### Author
Kenneth Onuma
