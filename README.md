# ASM-MathKit-x86-64-Assembly-Mathematical-Utilities

## Overview
This project consists of a collection of mathematical utilities implemented in x86-64 assembly language. The goal is to demonstrate the implementation of basic arithmetic operations and algorithms at a low level, providing insights into how such operations are handled at the assembly level.

## Features

### Modulo Operation
- **Functionality**: Calculates the remainder of division between two integers.
- **Method**: Continuously subtracts the divisor from the dividend until the remainder is less than the divisor.

### Greatest Common Divisor (GCD)
- **Functionality**: Finds the greatest common divisor of two numbers using the modulo method.
- **Method**: Recursively applies the modulo operation to reduce the problem size until the GCD is found.

### Prime Number Check
- **Functionality**: Determines whether a number is prime.
- **Method**: Utilizes the GCD method to check if the only divisors of the number are 1 and the number itself.

## Usage

To compile and run the assembly code, you will need an assembler and linker that supports x86-64 instructions. The GNU Assembler (GAS) is recommended. Here's how you can compile and run the program:

```bash
as -o math_utils.o math_utils.s
ld -o math_utils math_utils.o
./math_utils
