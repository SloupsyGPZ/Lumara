# Lumina Programming Language

A modern, elegant, and minimalist programming language designed for clarity and expressiveness, built from scratch.

## Language Features

- **Simple, clean syntax** inspired by Python and Rust
- **Static typing** with type inference
- **Functional and imperative programming paradigms**
- **Pattern matching** and algebraic data types
- **First-class functions** and closures
- **Module system** for code organization
- **Memory safety** with garbage collection
- **REPL** for interactive development

## Basic Syntax

```lumina
// Variable declaration with type inference
let name = "Lumina"
let version = 1.0

// Function definition
fn greet(name: str) -> str {
    return "Hello, {name}!"
}

// Pattern matching
fn describe_value(x) {
    match x {
        0 => "zero"
        1..10 => "small"
        _ => "large"
    }
}

// Struct definition
struct Person {
    name: str,
    age: i32
}

// Implementation block
impl Person {
    fn new(name: str, age: i32) -> Self {
        return Person { name, age }
    }
    
    fn greet(self) -> str {
        return "Hi, I'm {self.name} and I'm {self.age} years old."
    }
}
```

## Project Structure

```
lumina/
├── src/
│   ├── lexer.js          # Tokenizer
│   ├── parser.js         # AST parser
│   ├── interpreter.js    # Runtime interpreter
│   ├── repl.js           # REPL interface
│   └── main.js           # Entry point
├── examples/             # Example programs
├── tests/               # Test suite
└── package.json         # Node.js project file
```

## Building and Running

```bash
# Install dependencies
npm install

# Run the REPL
node src/main.js

# Run a Lumina file
node src/main.js examples/hello.lumina

# Run tests
npm test
```

## Development Status

This is the initial implementation of the Lumina programming language, built from scratch using JavaScript. The project includes:

- ✅ Lexer/tokenizer
- ✅ Parser with AST generation
- ✅ Basic interpreter
- ✅ REPL interface
- 🚄 Advanced type system
- 🚄 Standard library
- 🚄 Compiler backend (future)

## Architecture

The language is implemented with a clean separation of concerns:

1. **Lexer**: Converts source code into tokens
2. **Parser**: Builds abstract syntax trees from tokens
3. **Interpreter**: Executes the AST
4. **REPL**: Provides interactive development environment

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

# LICENCE 
Copyright (c) 2025 Lumara Project Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software.

# Trademark

The name "Lumara," the ".luma" file extension, and all associated branding are the intellectual property of the Lumara Project. While the source code is open source, the "Lumara" name may not be used for derivative programming languages without prior written authorization.
