# Monkey Interpreter

A tree-walking interpreter for the Monkey programming language, written in Go.

This project follows [Writing An Interpreter In Go](https://interpreterbook.com/) by Thorsten Ball.

## About

Built as a hands-on learning project to deepen my understanding of lexers, parsers, and tree-walking evaluation.

## About

Built as a hands-on learning project to deepen my understanding of lexers, parsers, and tree-walking evaluation.

## What is Monkey?

Monkey is a programming language designed specifically for learning about interpreters. It supports:

- Integer and boolean data types
- Strings
- Arrays and hash maps
- First-class functions and closures
- Higher-order functions
- A REPL (Read-Eval-Print Loop)

Here's a taste of what Monkey looks like:

```javascript
let fibonacci = fn(x) {
    if (x == 0) {
        return 0;
    }
    if (x == 1) {
        return 1;
    }
    return fibonacci(x - 1) + fibonacci(x - 2);
};

fibonacci(10);
```

## Future Project Structure

```
monkey-interpreter/
├── token/      # Token types and definitions
├── lexer/      # Lexical analysis (source code → tokens)
├── ast/        # Abstract syntax tree definitions
├── parser/     # Parsing (tokens → AST)
├── object/     # Object system for evaluation
├── evaluator/  # Tree-walking evaluation (AST → results)
└── repl/       # Interactive REPL
```

## Building and Running

```bash
# Run the REPL
go run main.go

# Run tests
go test ./...
```

## Progress

- [ ] Lexer
- [ ] Parser
- [ ] Evaluation
- [ ] Built-in functions
- [ ] Arrays and hashes

## Resources

- [Writing An Interpreter In Go](https://interpreterbook.com/)
- [The Lost Chapter: A Macro System](https://interpreterbook.com/lost/) — extending Monkey with macros