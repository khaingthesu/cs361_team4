# JAY Lexical Scanner & Recursive Descent Parser – CS361 Team 4

A lexical analyzer and recursive descent parser implemented in Java for the JAY language, developed by Khaing Su and Kevin Salgado Antonio.

## Overview
This project implements the scanner and parser stages for JAY based on the lexical syntax, EBNF concrete syntax, and abstract syntax. The scanner reads `.jay` input and produces Token objects (Value and Type), while the recursive descent parser validates syntax against JAY's grammar.

## Features
- Lexical Analysis (`Token.java`, `TokenStream.java`, `ScannerDemo.java`):
  - Recognizes JAY keywords, identifiers, integer and boolean literals , separators, and operators.
  - Skips whitespace and // comments .
  - Classifies unrecognized characters or invalid tokens as Other.
- Syntax Analysis (`ConcreteSyntax.java`, `ParserDemo.java`, `Program.java`):
  - Implements recursive descent parsing methods following the EBNF grammar rules for programs, declarations, statements, and expressions.
