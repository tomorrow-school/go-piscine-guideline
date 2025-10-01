# Go Piscine

This repository contains study guides and task notes for a multi-quest Go (Golang) piscine. Each quest builds practical skills step by step: from basic syntax and text processing to CLI tooling, data structures, and algorithms. The materials are organized so learners can quickly find what to study, how to structure solutions, and where to practice.

***

### What to expect

- Progressive difficulty: early quests focus on printing, strings, and control flow; mid quests cover slices, functions as values, file I/O, and CLI patterns; later quests introduce linked lists and binary search trees.
- Strict I/O formatting: outputs are validated by automated tests—pay close attention to whitespace, newlines, and exact messages.
- Manual implementations: many tasks forbid high-level helpers to deepen understanding (e.g., write substring search, atoi, sort, map/any/countif equivalents).
- Clean, idiomatic Go: prefer simple control flow, readable functions, and clear error handling.

***

### Skills by quest groups

- Text and numbers (Quests 2–5)
    - Printing runes and strings, recursion/iteration, basic math and conversions.
    - Manual string manipulation: substring search, concatenation, joining, rune-safe indexing.
    - Base conversions: print in base, parse with custom digit alphabets.
- CLI and files (Quest 6–8)
    - os.Args parsing, flags, ASCII sorting of args.
    - File I/O, stdin/stdout, building simplified cat/tail behavior.
    - Robust error messages and exit statuses.
- Functional patterns with slices (Quest 9)
    - Higher-order functions: ForEach, Map, Any, CountIf.
    - Custom sorting with comparators; arithmetic/doop with overflow checks.
- Data structures (Quests 11–12)
    - Singly linked lists: push front/back, size, last, at, reverse, foreach.
    - Binary search trees: insert, search, traversals (inorder, preorder, by-level), min/max, height, transplant, delete.

***

### How to work

- Read the task file fully before coding.
- Implement incrementally:
    - Start with the happy path, then add edge cases.
    - Add helper functions for repeated checks (e.g., base validity, rune class checks).
- Keep functions small and testable; avoid global state unless required.
- Favor clarity over cleverness. Use simple loops and conditionals.
- Validate all inputs:
    - For CLI: check argument count and flag combinations.
    - For strings: consider empty, whitespace-only, or non-ASCII inputs.
    - For numbers: overflow/underflow and division/modulo by zero.

***

### Testing locally

- Build small main.go drivers to test library functions in isolation.
- Compare outputs against the examples character-for-character.
- Test edge cases explicitly:
    - Empty inputs, single/rune boundaries, invalid bases, missing files, multiple files, large inputs.

***

### Style and structure

- Package layout
    - Library code in a dedicated package (e.g., piscine), main packages for test drivers.
- Naming
    - Use clear, lowerCamelCase for variables and functions; exported names only if required by the task.
- Error handling
    - Return values and errors as appropriate; when tasks require exact messages, print them precisely.
- Unicode safety
    - Use runes or range iteration for character operations; index bytes only when intended.

***

### Common pitfalls

- Treating bytes as characters: convert to []rune or iterate with range for Unicode correctness.
- Trailing separators: last element must not end with extra comma/space unless specified.
- Using disallowed helpers: respect constraints like “no make” or “no append.”
- Flag parsing vs plain args: parse flags before relying on positional arguments.
- Forgetting to handle nil/empty structures: linked list and tree tasks should guard on nil roots/nodes.

***

### Suggested workflow per task

1. Rephrase the requirement in one sentence to confirm understanding.
2. List constraints and edge cases (e.g., “no append,” “no make,” “ASCII order,” “nil if invalid range”).
3. Draft minimal pseudocode.
4. Implement and test with provided examples.
5. Add edge-case tests and compare outputs exactly.

***

### Learning and reference strategy

- Official documentation first for language features (spec, tour, by-example).
- Prioritize small, runnable examples to internalize concepts (I/O, runes, slices, maps).
- Keep a cheat sheet for:
    - Rune/byte differences
    - Slice creation/growth
    - Conversions (string↔int with bases)
    - CLI parsing patterns (flags vs raw args)
    - Linked list operations (head/tail invariants)
    - BST invariants (left < node < right, pointer updates)

***

### Contribution and maintenance

- Keep each quest’s README self-contained with:
    - Short concept overview
    - Key pitfalls
    - Minimal examples
    - Links to practice materials and docs
- When updating tasks:
    - Preserve original I/O contracts
    - Note any constraint changes prominently
    - Add new edge-case examples

***

### Feedback and Contact

- If any mistakes are spotted (grammar, technical details, links) or if improvements are suggested, please reach out to the authors on Telegram: @big_brother2998



