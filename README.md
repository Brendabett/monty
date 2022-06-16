
0x19. C - Stacks, Queues - LIFO, FIFO

# Monty

`monty` is an interpreter of Monty ByteCodes files, which is a scripting language just like Python.

## About the Monty language
This is a language that contains specific instructions to manipulate data information (stacks or queues), where each instruction (*called opcode*) is sended per line. Files which contains Monty byte codes usually have the `.m` extension.

## Technologies
* Interpreter was written with C language
* C files are compiled using `gcc 4.8.4`
* C files are written according to the C90 standard
* Tested on Ubuntu 20.04 LTS

## Usage
To compile all files:

```bash
$ gcc -Wall -Werror -Wextra -pedantic *.c -o monty
$
```

## Features
### Opcodes
`monty` executes the following opcodes:

| Opcode | Description |
| -------- | ----------- |
| `push` | Pushes an element to the stack |
| `pall` | Prints all the values on the stack |
| `pint` | Prints the value at the top of the stack |
| `pop` | Removes the top element of the stack |
| `swap` | Swaps the top two elements of the stack |
| `queue` | Sets the format of the data to a queue (FIFO) |
| `stack` | Sets the format of the data to a stack (LIFO) |
| `nop` | Doesn't do anything |
| `add` | Adds the top two elements of the stack |
| `sub` | Subtracts the top element of the stack from the second top element of the stack |
| `mul` | Multiplies the second top element of the stack with the top element of the stack |
| `div` | Divides the second top element of the stack by the top element of the stack |
| `mod` | Computes the rest of the division of the second top element of the stack by the top element of the stack |
| `pchar` | Prints the char at the top of the stack |
| `pstr` | Prints the string starting at the top of the stack |
| `rotl` | Rotates the stack to the top |
| `rotr` | Rotates the stack to the bottom |

Comments, indicated with `#`, are not executed by the interpreter.

### Return value
When there is no errors, `monty` returns `0`. Otherwise, returns `1`

## Authors

* Brenda Bett: [GitHub](https://github.com/Brendabett)
* Evans Kiprotich: [GitHub](https://github.com/KEvans254)
