# C-Like Language Compiler

This project is a C-like language compiler implemented using Flex (lexical analyzer) and Bison (parser generator) as part of a university project at the Computer Engineering and Informatics Department (CEID).

## Features

- Lexer: The Flex file (`flex.l`) contains the rules for tokenizing the input source code.
- Parser: The Bison file (`bison.y`) defines the grammar and rules for parsing the tokens generated by the lexer.
- Input Files: The input files (input.txt, input2.txt, input3.txt) contain correct grammar of the C-like language.
- Wrong Input File : The wronginput.txt file containt incorrect grammar of the C-like language.

## Language Constructs

The C-like language supported by the compiler includes the following constructs:

- Variables: Declare and use variables of integer and character types.
- Control Flow: Support for `if-else` statements, `while` and `for` loops, and `switch-case` statements.
- Functions: Define and call functions.
- Print Statement: Print statements using the `print` keyword.
- Comments: Support for single-line and multi-line comments.
- Data Types: Integer (`int`) and character (`char`) data types.
- Arrays: Declaration and usage of arrays.

## How to Run

To compile and run the C-like language compiler, follow these steps:

1. Install Flex and Bison: Ensure you have Flex and Bison installed on your system.
2. Compilation: Open a terminal, navigate to the project directory, and run the following commands:

```bash
flex lexer.l
bison -d parser.y
gcc lex.yy.c parser.tab.c -o compiler
