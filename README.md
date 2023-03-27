Collaborative C-PRINTF project with BELLO

DESCRIPTION

printf is a well known function used in C programming to do formated printing. Usually it only takes the standard library to call it into a c program, and using it for simple strings or formatted specifiers that allow us to print diferent types of data.
 This time we are presenting a printf project made from scratch in most of its features in order to understand the complexity of a powerful tool. You can see man 3 of printf to understand how _printf works.

COMPILATION

 gcc -Wall -Werror -Wextra -pedantic *.c

PROTOTYPE

int _printf(const char *format, ...)

RETURN

if the program runs successfully, it is to return the number of characters printed.

Header file: Main.h

Include all function prototypes
Include structure of specifiers

Project function: _printf
Start the variadic list.
Iterates string format of entry and check for a moldule symbol (%) . If the symbol is found then check if the next char match with one of the valid specifiers in the structure using the auxiliar function to comapare ( comp), in that case the respective function of these format is called.
For the characters that doesn't match any of the formats the function ignores the module symbole and print it as a string.
In case that the module symbole is not found, print the each character normally.

CONTRIBUTORS

KehindeAkinbowale
ziraabubakarbello
