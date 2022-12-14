This repository contains files on a C project, which requires ALX students to create the printf functions from scratch, as well as the man page for the functions

The project requires us to create various various standard library equivalents of printf in C, to _printf, a function which we will customize.

Function prototype: int _printf(const char *format, ...);

Examples
Integers

Input: _printf("We are %d\n", 2);
Output: We are 2
Characters

Input: _printf("Letter %c can be used to store an integer.\n", 'n');
Output: Letter n can be used to store an integer.
Strings

Input: _printf("%s\n", 'I am not tall.');
Output: I am not tall.
Decimals

Input: _printf("%d\n", 30);
Output: 30
Tasks
Mandatory ones

Write function that produces output with conversion specifiers c, s, and %.
Handle conversion specifiers d, i.
Create a man page for your function.
Advanced ones

Handle conversion specifier b.
Handle conversion specifiers u, o, x, X.
Use a local buffer of 1024 chars in order to call write as little as possible.
Handle conversion specifier S.
Handle conversion specifier p.
Handle flag characters +, space, and # for non-custom conversion specifiers.
Handle length modifiers l and h for non-custom conversion specifiers.
Handle the field width for non-custom conversion specifiers.
Handle the precision for non-custom conversion specifiers.
Handle the 0 flag character for non-custom conversion specifiers.
Handle the custom conversion specifier r that prints the reversed string.
Handle the custom conversion specifier R that prints the rot13'ed string.
All above options should work well together.
Files

_printf.c: - contains the function_printf, which uses the prototype int _printf(const char *format, ...);. The format string is composed of zero or more directives. See man 3 printf for more detail. _printf will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to stdout, the standard output stream.
_putchar.c: - contains the function _putchar, which writes a character to stdout.
holberton.h: - contains all function prototypes used for _printf.
man_3_printf: - manual page for the custom _printf function.
print_chars.c: - contains the functions print_c, print_s, print_S, and print_r which handle the conversion specifiers c, s, S, and r, respectively, as well as hex _print, which prints a char's ascii value in uppercase hex
print_numbers.c: - contains the functions print_i and print_d, which handle the conversion specifiers i and d, respectively
print_hex.c: - contains the functions print_hex, which prints an unsigned int in hexidecimal form, print_x, print_X, and print_p, which handle the conversion specifiers x, X, and p, respectively
print_unsigned_int.c: - contains the functions print_u, print_o, and print_b, which handle the conversion specifiers u, o, and b, respectively
print_rot13.c - contains the function print_R, which handles the conversion specifier R
