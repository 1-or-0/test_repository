# holbertonschool-printf

This repository contains the implementation of a custom `printf` function as part of the Holberton School curriculum.

## Table of Contents

- [Description](#description)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Files](#files)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

## Description

The project involves creating a custom `printf` function in C, mimicking the standard library's `printf` function. This function supports various format specifiers and flags.

## Requirements

- GCC (GNU Compiler Collection)
- C standard library
- Make

## Installation

Clone the repository:
```sh
git clone https://github.com/quliyevislam/holbertonschool-printf.git
```

Compile the code with your program:
```sh
gcc -Wall -Werror -Wextra -pedantic *.c -o your_program
```

## Usage

Include the header file in your C program:

```sh
#include "main.h"
```

Use the _printf function similar to the standard printf function:

```sh
_printf("Hello, %s!\n", "world");
```

Example Code

```sh
#include "main.h"int main(void)
{
    _printf("Character: %c\n", 'H');
    _printf("String: %s\n", "Hello, world!");
    _printf("Integer: %d\n", 42);
    _printf("Binary: %b\n", 5);
    _printf("Unsigned: %u\n", 12345);
    _printf("Octal: %o\n", 83);
    _printf("Hexadecimal: %x\n", 255);
    _printf("Pointer: %p\n", (void *)main);    return 0;
}
```

## Files

- README.md: This file.
- _printf.c: The main printf function implementation.
- _putchar.c: Helper function to write a character to stdout.
- main.h: Header file with function prototypes and macros.
- print_number.c: Functions to handle number printing.
- print_string.c: Functions to handle string printing.

## Testing

To test the _printf function, you can use the provided test cases or write your own. Ensure that your test cases cover various format specifiers and edge cases.

Example Test Code

```sh
#include <stdio.h>
#include "main.h"

int main(void)
{
    int len1, len2;    len1 = _printf("Character: %c\n", 'H');
    len2 = printf("Character: %c\n", 'H');
    printf("Custom printf length: %d, Standard printf length: %d\n", len1, len2);    len1 = _printf("String: %s\n", "Hello, world!");
    len2 = printf("String: %s\n", "Hello, world!");
    printf("Custom printf length: %d, Standard printf length: %d\n", len1, len2);    len1 = _printf("Integer: %d\n", 42);
    len2 = printf("Integer: %d\n", 42);
    printf("Custom printf length: %d, Standard printf length: %d\n", len1, len2);    return 0;
}
```

Compile and run the test code:

```sh
gcc -Wall -Werror -Wextra -pedantic *.c -o test_printf
./test_printf
```
Authors
Islam Quliyev quliyevislam
Orkhan Ibrahim OrkhanIbrahim357
