**Here is the updated documentation with all the equal-sign separators removed. This version uses standard bold headers and clean spacing, making it perfect for pasting into a professional document or a PDF.

LUMARA PROGRAMMING LANGUAGE SPECIFICATION Official Documentation and Project Roadmap Version 0.1.0 | 2025

1. PROJECT OVERVIEW Lumara is a high-level, tree-walking interpreted programming language engineered for structural integrity, expressive syntax, and architectural clarity. It is designed to bridge the gap between the flexibility of dynamic scripting and the rigid organization of systems-level data modeling.

Lumara utilizes a custom-built recursive descent parser and a scoped environment model to ensure memory safety and predictable execution.

2. LANGUAGE DESIGN PHILOSOPHY The development of Lumara is guided by three core pillars:

Explicit Structure: Data structures must be defined clearly, and behavior must be explicitly bound to those structures to prevent ambiguity.

Readable Complexity: Support for advanced features like nested closures and deep recursion without sacrificing the visual clarity of the source code.

Predictable Execution: A strict environment-based scoping model ensures memory safety and predictable variable resolution at runtime.

3. TECHNICAL ARCHITECTURE The Lumara runtime is divided into three distinct phases:

3.1 LEXICAL ANALYSIS (THE LEXER) The Lexer performs a linear scan of the .luma source file, converting raw characters into a stream of typed tokens. It handles whitespace sensitivity, literal detection (strings, numbers), and keyword identification.

3.2 SYNTACTIC ANALYSIS (THE PARSER) The Parser utilizes a recursive descent algorithm to transform the token stream into a hierarchical Abstract Syntax Tree (AST). This stage enforces the grammatical rules of Lumara and provides detailed error reporting.

3.3 RUNTIME EXECUTION (THE INTERPRETER) The Interpreter traverses the AST. It manages state using a nested Environment model, where each scope is a discrete memory map with a reference to its parent scope. This enables native support for lexical closures.

4. LANGUAGE SPECIFICATION

4.1 DATA TYPES

Number: 64-bit floating-point values.

String: UTF-8 encoded character sequences.

Boolean: true or false literals.

Struct: User-defined composite data types.

Function: First-class objects with lexical scoping.

4.2 BASIC SYNTAX let radius = 10 let pi = 3.14159

4.3 CONTROL FLOW if radius > 0 { print("Valid radius") } else { print("Invalid radius") }

4.4 FUNCTIONS AND CLOSURES fn multiplier(factor) { return fn (n) { return n * factor } } let triple = multiplier(3)

4.5 OBJECT-ORIENTED MODELING (STRUCTS & IMPLS) Data is structured using 'struct', and behavior is defined in 'impl' blocks. This separation ensures that logic remains modular and decoupled from data storage.

struct Player { name, health }

impl Player { fn heal(self, amount) { self.health = self.health + amount print(self.name, "healed to", self.health) } }

5. INSTALLATION AND USAGE

REQUIREMENTS:

Node.js v18.0 or higher

256MB RAM minimum

SETUP: git clone https://github.com/username/lumara.git cd lumara

EXECUTION: To start the REPL: node main.js To run a file: node main.js script.luma

6. DEVELOPMENT ROADMAP

v0.2.0: Standard Math and String library implementation.

v0.3.0: Integration of array primitives and iteration protocols.

v0.4.0: Introduction of a Foreign Function Interface (FFI).

v1.0.0: Stable release with optimized AST walking.

7. LICENSE AND INTELLECTUAL PROPERTY

SOFTWARE LICENSE: MIT Copyright (c) 2025 Lumara Project Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software.

TRADEMARK AND BRANDING: The name "Lumara," the ".luma" file extension, and all associated branding are the intellectual property of the Lumara Project. While the source code is open source, the "Lumara" name may not be used for derivative programming languages without prior written authorization.
**Lumara Programming Language Specification

Official Documentation and Project Roadmap
Version 0.1.0 | 2025

1. Project Overview

Lumara is a high-level, tree-walking interpreted programming language engineered for structural integrity, expressive syntax, and architectural clarity. It is designed to bridge the gap between the flexibility of dynamic scripting and the disciplined organization of systems-level data modeling.

Lumara uses a custom recursive-descent parser and a scoped environment model to ensure memory safety, lexical correctness, and predictable execution.

2. Language Design Philosophy

The development of Lumara is guided by three core principles:

Explicit Structure

Data structures must be clearly defined, and behavior must be explicitly bound to those structures to eliminate ambiguity.

Readable Complexity

The language supports advanced constructs such as nested closures and deep recursion while maintaining visual and conceptual clarity.

Predictable Execution

A strict, environment-based scoping model guarantees deterministic variable resolution and runtime safety.

3. Technical Architecture

The Lumara runtime is composed of three distinct phases:

3.1 Lexical Analysis (Lexer)

The lexer performs a linear scan of .luma source files, converting raw characters into a stream of typed tokens. It handles whitespace sensitivity, literal detection (numbers and strings), and keyword identification.

3.2 Syntactic Analysis (Parser)

The parser uses a recursive-descent algorithm to transform the token stream into a hierarchical Abstract Syntax Tree (AST). This phase enforces grammatical correctness and provides detailed syntax error reporting.

3.3 Runtime Execution (Interpreter)

The interpreter walks the AST and evaluates nodes using a nested Environment model. Each scope is an isolated memory map with a reference to its parent, enabling native lexical closures and safe variable resolution.

4. Language Specification
4.1 Data Types

Number — 64-bit floating-point values

String — UTF-8 encoded text

Boolean — true or false

Struct — User-defined composite data types

Function — First-class objects with lexical scoping

4.2 Basic Syntax
let radius = 10
let pi = 3.14159

4.3 Control Flow
if radius > 0 {
    print("Valid radius")
} else {
    print("Invalid radius")
}

4.4 Functions and Closures
fn multiplier(factor) {
    return fn (n) {
        return n * factor
    }
}

let triple = multiplier(3)

4.5 Object-Oriented Modeling (Structs & Impls)

Data is modeled using struct, while behavior is defined in impl blocks. This design enforces separation of concerns and promotes modular logic.

struct Player {
    name,
    health
}

impl Player {
    fn heal(self, amount) {
        self.health = self.health + amount
        print(self.name, "healed to", self.health)
    }
}

5. Installation and Usage
Requirements

Node.js v18.0 or higher

Minimum 256 MB RAM

Setup
git clone https://github.com/username/lumara.git
cd lumara

Execution

Start the REPL:

node main.js


Run a script:

node main.js script.luma

6. Development Roadmap

v0.2.0 — Standard math and string libraries

v0.3.0 — Array primitives and iteration protocols

v0.4.0 — Foreign Function Interface (FFI)

v1.0.0 — Stable release with optimized AST traversal

7. License and Intellectual Property
Software License

MIT License
Copyright © 2025 Lumara Project Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files to deal in the software without restriction, including the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies.

Trademark and Branding

The name “Lumara”, the .luma file extension, and all associated branding are the intellectual property of the Lumara Project. While the source code is open source, the Lumara name may not be used for derivative programming languages without prior written authorization.
