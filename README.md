# JAY Lexical Scanner & Recursive Descent Parser – CS361 Team 4

A lexical analyzer and recursive descent parser implemented in Java for the JAY language, developed by Khaing Su and Kevin Salgado Antonio.

## Overview
This project implements the scanner and parser stages for JAY based on the lexical syntax, EBNF concrete syntax, and abstract syntax. The scanner reads `.jay` input and produces Token objects (Value and Type), while the recursive descent parser validates syntax against JAY's grammar and creates the Abstract Syntax Tree (AST) or throws a syntax error.

## Features
- Lexical Analysis (`Token.java`, `TokenStream.java`, `ScannerDemo.java`):
  - Recognizes JAY keywords, identifiers, integer and boolean literals , separators, and operators.
  - Skips whitespace and // comments .
  - Classifies unrecognized characters or invalid tokens as Other.
- Syntax Analysis (`ConcreteSyntax.java`, `ParserDemo.java`, `Program.java`):
  - Implements recursive descent parsing methods following the EBNF grammar rules for programs, declarations, statements, and expressions.
  - Uses `Program.java` AST nodes to display the indented abstract syntax tree or report `Syntax error` exceptions on invalid syntax.
 
## Structure
```text
─ Token.java                  # Token representation (type and value)
─ TokenStream.java            # Lexical scanner for JAY input
─ ScannerDemo.java            # Program for printing scanner tokens
─ ConcreteSyntax.java         # Recursive descent parser implementation
─ ParserDemo.java             # Program for parsing and printing the AST
─ Program.java                # Abstract syntax tree definitions and display logic
─ prog1.jay                   # Scanner test cases
─ prog2.jay                   # Sample JAY program for parser testing
