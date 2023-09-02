# Lexical and Syntactical Analyzer

This Python application is designed to perform lexical and syntactical analysis on a given code file. It is composed of two main components: the lexical analyzer (lexer) and the syntactical analyzer (parser).

### Lexical Analysis
The lexical analyzer is responsible for breaking down the input code into smaller units called tokens. Each token represents a specific syntactical element in the code. The following token types are recognized:

- keyword: Represents the keyword "init".
- op: Represents operators such as "=", "+", "-", "*", and "/".
- int: Represents integer values.
- string: Represents string literals enclosed in double quotes.
- id: Represents identifiers, which are composed of letters, numbers, and underscores.
- eof: Represents the end of the file.

The lexical analysis is performed using a set of deterministic finite automata (DFAs) implemented in functions like afd_int, afd_string, and afd_identificador. These functions determine the type of token based on its content.

### Syntactical Analysis
The syntactical analyzer (parser) is responsible for verifying the correctness of the code's syntax. It ensures that the code follows a predefined grammar. The grammar rules checked by the parser are as follows:

A statement should consist of an identifier (id) followed by an operator (op) and an expression.
An expression (expr) consists of one or more terms, separated by addition or subtraction operators.
A term (term) can be either an integer (int) or an identifier (id).
If any syntax errors are detected during parsing, an exception is raised to indicate the presence of an error.

### How to Use
To use this application, follow these steps:

Create a text file (e.g., codigo.x) containing your code.
Open the file and write your code in it.
Run the Python script.
The code will be processed, and the lexer will generate a list of tokens.
The parser will then analyze the tokens and check for syntax errors.
If the code is syntactically correct, no errors will be raised. Otherwise, an exception will indicate the error and its location.
Ensure that you have Python installed on your system to run this application.

Example
You can use the codigo.x file, located in the repository.

## Developed by ⚙

<img src="https://avatars.githubusercontent.com/u/52716819?v=4" width="170"> | **Lucas de Abreu Furtado Garcia (https://github.com/Jornay)**<br> Developer/Student.<br> ||
