# Group _printf project

This file is a simple recreation of the printf function found in the stdio.h  header file.

It emulates the operation of the printf function which delivers an output according to a format composed by zero or more directives and conversion specifiers:

| Specifier | Output Produced
| ------ |------ |
| %c | Prints a character
| %s | Prints a string
| %% | Prints the % sign
| %d or %i | Prints numbers in decimal
| %u | Prints unsigned decimal
| %o | Prints numbers in octal
| %x | Prints in hexadecimal using lowercase abcdef
| %X | Prints in hexadecimal using uppercase ABCDEF
| %p | Prints pointer argumnet in hexadecimal
| l | Prints long int or unsigned long int
| h | Prints short int or unsigned short int

### The file equally contains some custom conversion specifiers

| Custom Specifier | Output Produced
| --- | --- |
| %b |  An unsigned int argument, **converted to binary**
| %S | Prints a string *but* Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)
| %r | Prints a string but in reverse
| %R | Prints a rot13'ed string

### It also handles a few flag characters

- '+' flag
- 'space' flag
- '#' flag
- '0' flag
- '-' flag

## Other things handled in the file: 

- Field width
- Precision
