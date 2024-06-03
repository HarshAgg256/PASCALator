# PASCALator
A compiler for simplified PASCAL language

## Overview 

This project is an implementation of a basic PASCAL compiler which supports the following features of the basic PASCAL programming language:

- Integer constants
- Keywords
- Variables
- Expressions
- Assignments
- Conditional statements
- Loops
- Arrays
- Single line comments (using //)
- Read and Write statements
  
The project is divided into several phases: Lexical Analysis, Syntax Analysis, Semantic Analysis, Code Generation, and Final Output Generation. Each phase builds upon the previous one to construct a fully functional compiler.

### Language Specification
The language specification includes the definition and syntax for:

**Keywords**: A list of reserved words in PASCAL (e.g., program, var, integer, real, boolean, char, if, else, while, for, do, array, begin, end, read, write).<br>
**Variables/Identifiers**: Rules for variable names and their declarations.<br>
**Operators**: Supported arithmetic, relational, and boolean operators.<br>
**Statements**: Including read/write statements, assignment statements, blocks of statements, conditional statements, and looping statements.<br>
**Program Structure**: The overall structure of a PASCAL program, including the program keyword, variable declarations, and the main program block.<br>

### Tasks

*Part-1: Lexical and Syntax Analysis*

**Lexical Analysis**:

Developed a LEX program to tokenize the input PASCAL program into identifiers, operators, numbers, keywords, punctuators, etc.

**Syntax Analysis**:

Developed a YACC program to parse the tokens generated from the lexical analysis phase and check the syntax of the input program. A symbol table is created at this stage, although it is not required to be printed.

*Part-2: Semantic Analysis, Code Generation, and Final Output*

**Semantic Analysis**:

Extended the YACC program to check for semantic errors and generate an Abstract Syntax Tree (AST). Semantic errors include type checking, undeclared variables, multiple declarations, and using variables before assignment.

**Code Generation**:

Extended the YACC program to generate intermediate code in three-address code format.

**Final Stage**:

Extended the YACC program to print the output of the input program and display the symbol table.

*Task-specific Output:*

**Lexical Analysis**: The list of valid tokens in the format: line number lexeme token type.<br>
**Syntax Analysis**: If the input program has no syntax errors, valid input is displayed. Otherwise, syntax error is displayed.<br>
**Semantic Analysis**: The AST is displayed. If there are semantic errors, appropriate error messages are displayed such as undeclared variable, multiple declarations of a variable, and type mismatches.<br>
**Code Generation**: The generated three-address code is displayed.<br>
**Final Stage**: The output of the given input program and the symbol table are displayed in the format: Variable Type Value.<br>
